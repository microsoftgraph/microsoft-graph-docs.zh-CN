---
title: 创建 windows10GeneralConfiguration
description: 创建新的 windows10GeneralConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 378056d369be75fec3654d7206927250a8914205
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757036"
---
# <a name="create-windows10generalconfiguration"></a><span data-ttu-id="cd825-103">创建 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd825-103">Create windows10GeneralConfiguration</span></span>

<span data-ttu-id="cd825-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd825-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd825-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd825-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd825-106">创建新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd825-106">Create a new [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd825-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd825-107">Prerequisites</span></span>
<span data-ttu-id="cd825-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd825-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd825-110">Permission type</span></span>|<span data-ttu-id="cd825-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd825-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd825-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd825-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd825-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd825-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cd825-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd825-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd825-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd825-115">Not supported.</span></span>|
|<span data-ttu-id="cd825-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd825-116">Application</span></span>|<span data-ttu-id="cd825-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd825-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd825-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd825-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cd825-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd825-119">Request headers</span></span>
|<span data-ttu-id="cd825-120">标头</span><span class="sxs-lookup"><span data-stu-id="cd825-120">Header</span></span>|<span data-ttu-id="cd825-121">值</span><span class="sxs-lookup"><span data-stu-id="cd825-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd825-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd825-122">Authorization</span></span>|<span data-ttu-id="cd825-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd825-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd825-124">接受</span><span class="sxs-lookup"><span data-stu-id="cd825-124">Accept</span></span>|<span data-ttu-id="cd825-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd825-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd825-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd825-126">Request body</span></span>
<span data-ttu-id="cd825-127">在请求正文中，提供 windows10GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd825-127">In the request body, supply a JSON representation for the windows10GeneralConfiguration object.</span></span>

<span data-ttu-id="cd825-128">下表显示了创建 windows10GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cd825-128">The following table shows the properties that are required when you create the windows10GeneralConfiguration.</span></span>

|<span data-ttu-id="cd825-129">属性</span><span class="sxs-lookup"><span data-stu-id="cd825-129">Property</span></span>|<span data-ttu-id="cd825-130">类型</span><span class="sxs-lookup"><span data-stu-id="cd825-130">Type</span></span>|<span data-ttu-id="cd825-131">说明</span><span class="sxs-lookup"><span data-stu-id="cd825-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd825-132">id</span><span class="sxs-lookup"><span data-stu-id="cd825-132">id</span></span>|<span data-ttu-id="cd825-133">String</span><span class="sxs-lookup"><span data-stu-id="cd825-133">String</span></span>|<span data-ttu-id="cd825-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cd825-134">Key of the entity.</span></span> <span data-ttu-id="cd825-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd825-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd825-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd825-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cd825-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd825-137">DateTimeOffset</span></span>|<span data-ttu-id="cd825-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cd825-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cd825-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd825-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd825-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd825-140">createdDateTime</span></span>|<span data-ttu-id="cd825-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd825-141">DateTimeOffset</span></span>|<span data-ttu-id="cd825-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cd825-142">DateTime the object was created.</span></span> <span data-ttu-id="cd825-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd825-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd825-144">说明</span><span class="sxs-lookup"><span data-stu-id="cd825-144">description</span></span>|<span data-ttu-id="cd825-145">String</span><span class="sxs-lookup"><span data-stu-id="cd825-145">String</span></span>|<span data-ttu-id="cd825-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="cd825-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cd825-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd825-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd825-148">displayName</span><span class="sxs-lookup"><span data-stu-id="cd825-148">displayName</span></span>|<span data-ttu-id="cd825-149">String</span><span class="sxs-lookup"><span data-stu-id="cd825-149">String</span></span>|<span data-ttu-id="cd825-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="cd825-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cd825-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd825-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd825-152">version</span><span class="sxs-lookup"><span data-stu-id="cd825-152">version</span></span>|<span data-ttu-id="cd825-153">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-153">Int32</span></span>|<span data-ttu-id="cd825-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="cd825-154">Version of the device configuration.</span></span> <span data-ttu-id="cd825-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd825-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd825-156">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="cd825-156">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="cd825-157">String</span><span class="sxs-lookup"><span data-stu-id="cd825-157">String</span></span>|<span data-ttu-id="cd825-158">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="cd825-158">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="cd825-159">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="cd825-159">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="cd825-160">String</span><span class="sxs-lookup"><span data-stu-id="cd825-160">String</span></span>|<span data-ttu-id="cd825-161">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="cd825-161">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="cd825-162">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="cd825-162">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="cd825-163">String</span><span class="sxs-lookup"><span data-stu-id="cd825-163">String</span></span>|<span data-ttu-id="cd825-164">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="cd825-164">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="cd825-165">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cd825-165">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="cd825-166">String</span><span class="sxs-lookup"><span data-stu-id="cd825-166">String</span></span>|<span data-ttu-id="cd825-167">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="cd825-167">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="cd825-168">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="cd825-168">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="cd825-169">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-169">Int32</span></span>|<span data-ttu-id="cd825-170">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="cd825-170">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="cd825-171">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="cd825-171">This is a mobile only setting.</span></span> <span data-ttu-id="cd825-172">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="cd825-172">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="cd825-173">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cd825-173">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="cd825-174">String</span><span class="sxs-lookup"><span data-stu-id="cd825-174">String</span></span>|<span data-ttu-id="cd825-175">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="cd825-175">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="cd825-176">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="cd825-176">searchBlockDiacritics</span></span>|<span data-ttu-id="cd825-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-177">Boolean</span></span>|<span data-ttu-id="cd825-178">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="cd825-178">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="cd825-179">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="cd825-179">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="cd825-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-180">Boolean</span></span>|<span data-ttu-id="cd825-181">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="cd825-181">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="cd825-182">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="cd825-182">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="cd825-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-183">Boolean</span></span>|<span data-ttu-id="cd825-184">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="cd825-184">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="cd825-185">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="cd825-185">searchEnableRemoteQueries</span></span>|<span data-ttu-id="cd825-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-186">Boolean</span></span>|<span data-ttu-id="cd825-187">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="cd825-187">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="cd825-188">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="cd825-188">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="cd825-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-189">Boolean</span></span>|<span data-ttu-id="cd825-190">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="cd825-190">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="cd825-191">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="cd825-191">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="cd825-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-192">Boolean</span></span>|<span data-ttu-id="cd825-193">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="cd825-193">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="cd825-194">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="cd825-194">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="cd825-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-195">Boolean</span></span>|<span data-ttu-id="cd825-196">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="cd825-196">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="cd825-197">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="cd825-197">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="cd825-198">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="cd825-198">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="cd825-199">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="cd825-199">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="cd825-200">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="cd825-200">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="cd825-201">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="cd825-201">oneDriveDisableFileSync</span></span>|<span data-ttu-id="cd825-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-202">Boolean</span></span>|<span data-ttu-id="cd825-203">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="cd825-203">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="cd825-204">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="cd825-204">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="cd825-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-205">Boolean</span></span>|<span data-ttu-id="cd825-206">此属性将在 2019 年 7 月弃用，并替换为属性 SmartScreenAppInstallControl。</span><span class="sxs-lookup"><span data-stu-id="cd825-206">This property will be deprecated in July 2019 and will be replaced by property SmartScreenAppInstallControl.</span></span> <span data-ttu-id="cd825-207">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="cd825-207">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="cd825-208">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="cd825-208">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="cd825-209">String</span><span class="sxs-lookup"><span data-stu-id="cd825-209">String</span></span>|<span data-ttu-id="cd825-210">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="cd825-210">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="cd825-211">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="cd825-211">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="cd825-212">String</span><span class="sxs-lookup"><span data-stu-id="cd825-212">String</span></span>|<span data-ttu-id="cd825-213">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="cd825-213">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="cd825-214">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="cd825-214">bluetoothAllowedServices</span></span>|<span data-ttu-id="cd825-215">String 集合</span><span class="sxs-lookup"><span data-stu-id="cd825-215">String collection</span></span>|<span data-ttu-id="cd825-216">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="cd825-216">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="cd825-217">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="cd825-217">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="cd825-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-218">Boolean</span></span>|<span data-ttu-id="cd825-219">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="cd825-219">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="cd825-220">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="cd825-220">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="cd825-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-221">Boolean</span></span>|<span data-ttu-id="cd825-222">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="cd825-222">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="cd825-223">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="cd825-223">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="cd825-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-224">Boolean</span></span>|<span data-ttu-id="cd825-225">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="cd825-225">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="cd825-226">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="cd825-226">edgeBlockAutofill</span></span>|<span data-ttu-id="cd825-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-227">Boolean</span></span>|<span data-ttu-id="cd825-228">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="cd825-228">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="cd825-229">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-229">edgeBlocked</span></span>|<span data-ttu-id="cd825-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-230">Boolean</span></span>|<span data-ttu-id="cd825-231">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="cd825-231">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="cd825-232">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="cd825-232">edgeCookiePolicy</span></span>|[<span data-ttu-id="cd825-233">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="cd825-233">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="cd825-234">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="cd825-234">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="cd825-235">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="cd825-235">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="cd825-236">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="cd825-236">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="cd825-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-237">Boolean</span></span>|<span data-ttu-id="cd825-238">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="cd825-238">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="cd825-239">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="cd825-239">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="cd825-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-240">Boolean</span></span>|<span data-ttu-id="cd825-241">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="cd825-241">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="cd825-242">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="cd825-242">edgeBlockExtensions</span></span>|<span data-ttu-id="cd825-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-243">Boolean</span></span>|<span data-ttu-id="cd825-244">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="cd825-244">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="cd825-245">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="cd825-245">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="cd825-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-246">Boolean</span></span>|<span data-ttu-id="cd825-247">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="cd825-247">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="cd825-248">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="cd825-248">edgeBlockJavaScript</span></span>|<span data-ttu-id="cd825-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-249">Boolean</span></span>|<span data-ttu-id="cd825-250">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="cd825-250">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="cd825-251">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="cd825-251">edgeBlockPasswordManager</span></span>|<span data-ttu-id="cd825-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-252">Boolean</span></span>|<span data-ttu-id="cd825-253">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="cd825-253">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="cd825-254">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="cd825-254">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="cd825-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-255">Boolean</span></span>|<span data-ttu-id="cd825-256">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="cd825-256">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="cd825-257">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="cd825-257">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="cd825-258">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="cd825-258">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="cd825-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-259">Boolean</span></span>|<span data-ttu-id="cd825-260">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="cd825-260">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="cd825-261">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="cd825-261">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="cd825-262">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="cd825-262">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="cd825-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-263">Boolean</span></span>|<span data-ttu-id="cd825-264">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="cd825-264">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="cd825-265">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="cd825-265">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="cd825-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-266">Boolean</span></span>|<span data-ttu-id="cd825-267">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="cd825-267">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="cd825-268">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="cd825-268">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="cd825-269">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="cd825-269">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="cd825-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-270">Boolean</span></span>|<span data-ttu-id="cd825-271">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="cd825-271">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="cd825-272">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="cd825-272">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="cd825-273">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="cd825-273">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="cd825-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-274">Boolean</span></span>|<span data-ttu-id="cd825-275">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="cd825-275">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="cd825-276">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="cd825-276">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="cd825-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-277">Boolean</span></span>|<span data-ttu-id="cd825-278">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="cd825-278">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="cd825-279">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="cd825-279">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="cd825-280">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="cd825-280">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="cd825-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-281">Boolean</span></span>|<span data-ttu-id="cd825-282">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="cd825-282">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="cd825-283">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="cd825-283">cellularBlockVpn</span></span>|<span data-ttu-id="cd825-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-284">Boolean</span></span>|<span data-ttu-id="cd825-285">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="cd825-285">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="cd825-286">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="cd825-286">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="cd825-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-287">Boolean</span></span>|<span data-ttu-id="cd825-288">通过手机网络漫游时是否阻止用户使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="cd825-288">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="cd825-289">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="cd825-289">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="cd825-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-290">Boolean</span></span>|<span data-ttu-id="cd825-291">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="cd825-291">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="cd825-292">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="cd825-292">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="cd825-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-293">Boolean</span></span>|<span data-ttu-id="cd825-294">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="cd825-294">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="cd825-295">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="cd825-295">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="cd825-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-296">Boolean</span></span>|<span data-ttu-id="cd825-297">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="cd825-297">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="cd825-298">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="cd825-298">defenderScanDownloads</span></span>|<span data-ttu-id="cd825-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-299">Boolean</span></span>|<span data-ttu-id="cd825-300">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="cd825-300">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="cd825-301">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="cd825-301">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="cd825-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-302">Boolean</span></span>|<span data-ttu-id="cd825-303">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="cd825-303">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="cd825-304">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="cd825-304">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="cd825-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-305">Boolean</span></span>|<span data-ttu-id="cd825-306">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="cd825-306">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="cd825-307">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="cd825-307">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="cd825-308">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-308">Int32</span></span>|<span data-ttu-id="cd825-309">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="cd825-309">The signature update interval in hours.</span></span> <span data-ttu-id="cd825-310">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="cd825-310">Specify 0 not to check.</span></span> <span data-ttu-id="cd825-311">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="cd825-311">Valid values 0 to 24</span></span>|
|<span data-ttu-id="cd825-312">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="cd825-312">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="cd825-313">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="cd825-313">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="cd825-314">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="cd825-314">Value for monitoring file activity.</span></span> <span data-ttu-id="cd825-315">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="cd825-315">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="cd825-316">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="cd825-316">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="cd825-317">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-317">Int32</span></span>|<span data-ttu-id="cd825-318">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="cd825-318">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="cd825-319">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="cd825-319">Valid values 0 to 90</span></span>|
|<span data-ttu-id="cd825-320">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="cd825-320">defenderScanMaxCpu</span></span>|<span data-ttu-id="cd825-321">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-321">Int32</span></span>|<span data-ttu-id="cd825-322">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="cd825-322">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="cd825-323">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="cd825-323">Valid values 0 to 100</span></span>|
|<span data-ttu-id="cd825-324">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="cd825-324">defenderScanArchiveFiles</span></span>|<span data-ttu-id="cd825-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-325">Boolean</span></span>|<span data-ttu-id="cd825-326">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="cd825-326">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="cd825-327">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="cd825-327">defenderScanIncomingMail</span></span>|<span data-ttu-id="cd825-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-328">Boolean</span></span>|<span data-ttu-id="cd825-329">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="cd825-329">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="cd825-330">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="cd825-330">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="cd825-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-331">Boolean</span></span>|<span data-ttu-id="cd825-332">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="cd825-332">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="cd825-333">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="cd825-333">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="cd825-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-334">Boolean</span></span>|<span data-ttu-id="cd825-335">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="cd825-335">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="cd825-336">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="cd825-336">defenderScanNetworkFiles</span></span>|<span data-ttu-id="cd825-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-337">Boolean</span></span>|<span data-ttu-id="cd825-338">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="cd825-338">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="cd825-339">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="cd825-339">defenderRequireCloudProtection</span></span>|<span data-ttu-id="cd825-340">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-340">Boolean</span></span>|<span data-ttu-id="cd825-341">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="cd825-341">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="cd825-342">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="cd825-342">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="cd825-343">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="cd825-343">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="cd825-344">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="cd825-344">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="cd825-345">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="cd825-345">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="cd825-346">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="cd825-346">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="cd825-347">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="cd825-347">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="cd825-348">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="cd825-348">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="cd825-349">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="cd825-349">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="cd825-350">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="cd825-350">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="cd825-351">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cd825-351">TimeOfDay</span></span>|<span data-ttu-id="cd825-352">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="cd825-352">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="cd825-353">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="cd825-353">defenderScanType</span></span>|[<span data-ttu-id="cd825-354">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="cd825-354">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="cd825-355">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="cd825-355">The defender system scan type.</span></span> <span data-ttu-id="cd825-356">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="cd825-356">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="cd825-357">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="cd825-357">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="cd825-358">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="cd825-358">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="cd825-359">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="cd825-359">Defender day of the week for the system scan.</span></span> <span data-ttu-id="cd825-360">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="cd825-360">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="cd825-361">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="cd825-361">defenderScheduledScanTime</span></span>|<span data-ttu-id="cd825-362">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cd825-362">TimeOfDay</span></span>|<span data-ttu-id="cd825-363">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="cd825-363">The defender time for the system scan.</span></span>|
|<span data-ttu-id="cd825-364">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="cd825-364">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="cd825-365">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="cd825-365">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="cd825-366">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="cd825-366">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="cd825-367">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="cd825-367">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="cd825-368">String 集合</span><span class="sxs-lookup"><span data-stu-id="cd825-368">String collection</span></span>|<span data-ttu-id="cd825-369">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="cd825-369">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="cd825-370">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="cd825-370">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="cd825-371">String 集合</span><span class="sxs-lookup"><span data-stu-id="cd825-371">String collection</span></span>|<span data-ttu-id="cd825-372">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="cd825-372">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="cd825-373">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="cd825-373">defenderProcessesToExclude</span></span>|<span data-ttu-id="cd825-374">String 集合</span><span class="sxs-lookup"><span data-stu-id="cd825-374">String collection</span></span>|<span data-ttu-id="cd825-375">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="cd825-375">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="cd825-376">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd825-376">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="cd825-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-377">Boolean</span></span>|<span data-ttu-id="cd825-378">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="cd825-378">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="cd825-379">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="cd825-379">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="cd825-380">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="cd825-380">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="cd825-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-381">Boolean</span></span>|<span data-ttu-id="cd825-382">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="cd825-382">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="cd825-383">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="cd825-383">lockScreenBlockCortana</span></span>|<span data-ttu-id="cd825-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-384">Boolean</span></span>|<span data-ttu-id="cd825-385">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="cd825-385">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="cd825-386">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="cd825-386">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="cd825-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-387">Boolean</span></span>|<span data-ttu-id="cd825-388">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="cd825-388">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="cd825-389">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="cd825-389">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="cd825-390">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-390">Int32</span></span>|<span data-ttu-id="cd825-391">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="cd825-391">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="cd825-392">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="cd825-392">Supported values are 11-1800.</span></span> <span data-ttu-id="cd825-393">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="cd825-393">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="cd825-394">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="cd825-394">passwordBlockSimple</span></span>|<span data-ttu-id="cd825-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-395">Boolean</span></span>|<span data-ttu-id="cd825-396">指定是否允许使用 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="cd825-396">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="cd825-397">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="cd825-397">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="cd825-398">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cd825-398">passwordExpirationDays</span></span>|<span data-ttu-id="cd825-399">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-399">Int32</span></span>|<span data-ttu-id="cd825-400">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="cd825-400">The password expiration in days.</span></span> <span data-ttu-id="cd825-401">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="cd825-401">Valid values 0 to 730</span></span>|
|<span data-ttu-id="cd825-402">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cd825-402">passwordMinimumLength</span></span>|<span data-ttu-id="cd825-403">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-403">Int32</span></span>|<span data-ttu-id="cd825-404">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="cd825-404">The minimum password length.</span></span> <span data-ttu-id="cd825-405">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="cd825-405">Valid values 4 to 16</span></span>|
|<span data-ttu-id="cd825-406">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="cd825-406">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="cd825-407">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-407">Int32</span></span>|<span data-ttu-id="cd825-408">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="cd825-408">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="cd825-409">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="cd825-409">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="cd825-410">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-410">Int32</span></span>|<span data-ttu-id="cd825-411">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="cd825-411">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="cd825-412">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="cd825-412">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="cd825-413">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-413">Int32</span></span>|<span data-ttu-id="cd825-414">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="cd825-414">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="cd825-415">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="cd825-415">Valid values 0 to 50</span></span>|
|<span data-ttu-id="cd825-416">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="cd825-416">passwordRequired</span></span>|<span data-ttu-id="cd825-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-417">Boolean</span></span>|<span data-ttu-id="cd825-418">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="cd825-418">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="cd825-419">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="cd825-419">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="cd825-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-420">Boolean</span></span>|<span data-ttu-id="cd825-421">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="cd825-421">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="cd825-422">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cd825-422">passwordRequiredType</span></span>|[<span data-ttu-id="cd825-423">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cd825-423">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="cd825-424">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="cd825-424">The required password type.</span></span> <span data-ttu-id="cd825-425">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="cd825-425">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="cd825-426">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="cd825-426">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="cd825-427">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-427">Int32</span></span>|<span data-ttu-id="cd825-428">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="cd825-428">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="cd825-429">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="cd825-429">Valid values 0 to 999</span></span>|
|<span data-ttu-id="cd825-430">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="cd825-430">privacyAdvertisingId</span></span>|[<span data-ttu-id="cd825-431">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="cd825-431">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="cd825-432">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="cd825-432">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="cd825-433">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="cd825-433">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="cd825-434">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="cd825-434">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="cd825-435">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="cd825-435">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="cd825-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-436">Boolean</span></span>|<span data-ttu-id="cd825-437">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="cd825-437">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="cd825-438">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="cd825-438">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="cd825-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-439">Boolean</span></span>|<span data-ttu-id="cd825-440">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="cd825-440">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="cd825-441">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="cd825-441">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="cd825-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-442">Boolean</span></span>|<span data-ttu-id="cd825-443">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="cd825-443">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="cd825-444">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="cd825-444">startMenuAppListVisibility</span></span>|[<span data-ttu-id="cd825-445">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="cd825-445">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="cd825-446">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="cd825-446">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="cd825-447">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="cd825-447">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="cd825-448">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="cd825-448">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="cd825-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-449">Boolean</span></span>|<span data-ttu-id="cd825-450">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="cd825-450">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="cd825-451">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="cd825-451">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="cd825-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-452">Boolean</span></span>|<span data-ttu-id="cd825-453">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="cd825-453">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="cd825-454">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="cd825-454">startMenuHideHibernate</span></span>|<span data-ttu-id="cd825-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-455">Boolean</span></span>|<span data-ttu-id="cd825-456">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="cd825-456">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="cd825-457">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="cd825-457">startMenuHideLock</span></span>|<span data-ttu-id="cd825-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-458">Boolean</span></span>|<span data-ttu-id="cd825-459">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="cd825-459">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="cd825-460">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="cd825-460">startMenuHidePowerButton</span></span>|<span data-ttu-id="cd825-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-461">Boolean</span></span>|<span data-ttu-id="cd825-462">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="cd825-462">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="cd825-463">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="cd825-463">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="cd825-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-464">Boolean</span></span>|<span data-ttu-id="cd825-465">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="cd825-465">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="cd825-466">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="cd825-466">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="cd825-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-467">Boolean</span></span>|<span data-ttu-id="cd825-468">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="cd825-468">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="cd825-469">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="cd825-469">startMenuHideRestartOptions</span></span>|<span data-ttu-id="cd825-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-470">Boolean</span></span>|<span data-ttu-id="cd825-471">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="cd825-471">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="cd825-472">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="cd825-472">startMenuHideShutDown</span></span>|<span data-ttu-id="cd825-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-473">Boolean</span></span>|<span data-ttu-id="cd825-474">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="cd825-474">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="cd825-475">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="cd825-475">startMenuHideSignOut</span></span>|<span data-ttu-id="cd825-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-476">Boolean</span></span>|<span data-ttu-id="cd825-477">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="cd825-477">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="cd825-478">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="cd825-478">startMenuHideSleep</span></span>|<span data-ttu-id="cd825-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-479">Boolean</span></span>|<span data-ttu-id="cd825-480">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="cd825-480">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="cd825-481">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="cd825-481">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="cd825-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-482">Boolean</span></span>|<span data-ttu-id="cd825-483">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="cd825-483">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="cd825-484">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="cd825-484">startMenuHideUserTile</span></span>|<span data-ttu-id="cd825-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-485">Boolean</span></span>|<span data-ttu-id="cd825-486">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="cd825-486">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="cd825-487">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="cd825-487">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="cd825-488">Binary</span><span class="sxs-lookup"><span data-stu-id="cd825-488">Binary</span></span>|<span data-ttu-id="cd825-489">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="cd825-489">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="cd825-490">“开始”菜单布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="cd825-490">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="cd825-491">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="cd825-491">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="cd825-492">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="cd825-492">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="cd825-493">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="cd825-493">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="cd825-494">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="cd825-494">startMenuLayoutXml</span></span>|<span data-ttu-id="cd825-495">Binary</span><span class="sxs-lookup"><span data-stu-id="cd825-495">Binary</span></span>|<span data-ttu-id="cd825-496">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="cd825-496">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="cd825-497">通过基于布局修改架构指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="cd825-497">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="cd825-498">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="cd825-498">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="cd825-499">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="cd825-499">startMenuMode</span></span>|[<span data-ttu-id="cd825-500">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="cd825-500">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="cd825-501">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="cd825-501">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="cd825-502">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="cd825-502">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="cd825-503">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="cd825-503">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="cd825-504">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="cd825-504">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="cd825-505">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="cd825-505">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="cd825-506">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="cd825-506">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="cd825-507">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="cd825-507">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="cd825-508">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="cd825-508">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="cd825-509">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="cd825-509">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="cd825-510">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="cd825-510">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="cd825-511">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="cd825-511">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="cd825-512">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="cd825-512">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="cd825-513">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="cd825-513">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="cd825-514">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="cd825-514">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="cd825-515">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="cd825-515">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="cd825-516">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="cd825-516">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="cd825-517">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="cd825-517">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="cd825-518">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="cd825-518">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="cd825-519">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="cd825-519">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="cd825-520">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="cd825-520">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="cd825-521">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="cd825-521">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="cd825-522">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="cd825-522">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="cd825-523">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="cd825-523">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="cd825-524">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="cd825-524">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="cd825-525">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="cd825-525">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="cd825-526">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="cd825-526">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="cd825-527">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="cd825-527">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="cd825-528">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="cd825-528">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="cd825-529">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="cd825-529">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="cd825-530">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="cd825-530">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="cd825-531">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="cd825-531">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="cd825-532">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="cd825-532">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="cd825-533">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="cd825-533">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="cd825-534">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="cd825-534">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="cd825-535">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="cd825-535">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="cd825-536">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="cd825-536">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="cd825-537">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="cd825-537">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="cd825-538">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="cd825-538">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="cd825-539">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="cd825-539">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="cd825-540">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="cd825-540">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="cd825-541">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="cd825-541">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="cd825-542">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="cd825-542">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="cd825-543">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="cd825-543">settingsBlockSettingsApp</span></span>|<span data-ttu-id="cd825-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-544">Boolean</span></span>|<span data-ttu-id="cd825-545">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="cd825-545">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="cd825-546">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="cd825-546">settingsBlockSystemPage</span></span>|<span data-ttu-id="cd825-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-547">Boolean</span></span>|<span data-ttu-id="cd825-548">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="cd825-548">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="cd825-549">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="cd825-549">settingsBlockDevicesPage</span></span>|<span data-ttu-id="cd825-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-550">Boolean</span></span>|<span data-ttu-id="cd825-551">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="cd825-551">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="cd825-552">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="cd825-552">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="cd825-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-553">Boolean</span></span>|<span data-ttu-id="cd825-554">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="cd825-554">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="cd825-555">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="cd825-555">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="cd825-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-556">Boolean</span></span>|<span data-ttu-id="cd825-557">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="cd825-557">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="cd825-558">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="cd825-558">settingsBlockAccountsPage</span></span>|<span data-ttu-id="cd825-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-559">Boolean</span></span>|<span data-ttu-id="cd825-560">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="cd825-560">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="cd825-561">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="cd825-561">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="cd825-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-562">Boolean</span></span>|<span data-ttu-id="cd825-563">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="cd825-563">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="cd825-564">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="cd825-564">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="cd825-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-565">Boolean</span></span>|<span data-ttu-id="cd825-566">指示是否阻止在“设置”应用中访问“轻松使用”。</span><span class="sxs-lookup"><span data-stu-id="cd825-566">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="cd825-567">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="cd825-567">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="cd825-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-568">Boolean</span></span>|<span data-ttu-id="cd825-569">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="cd825-569">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="cd825-570">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="cd825-570">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="cd825-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-571">Boolean</span></span>|<span data-ttu-id="cd825-572">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="cd825-572">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="cd825-573">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="cd825-573">settingsBlockAppsPage</span></span>|<span data-ttu-id="cd825-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-574">Boolean</span></span>|<span data-ttu-id="cd825-575">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="cd825-575">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="cd825-576">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="cd825-576">settingsBlockGamingPage</span></span>|<span data-ttu-id="cd825-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-577">Boolean</span></span>|<span data-ttu-id="cd825-578">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="cd825-578">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="cd825-579">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="cd825-579">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="cd825-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-580">Boolean</span></span>|<span data-ttu-id="cd825-581">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="cd825-581">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="cd825-582">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-582">windowsSpotlightBlocked</span></span>|<span data-ttu-id="cd825-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-583">Boolean</span></span>|<span data-ttu-id="cd825-584">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="cd825-584">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="cd825-585">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="cd825-585">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="cd825-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-586">Boolean</span></span>|<span data-ttu-id="cd825-587">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="cd825-587">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="cd825-588">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="cd825-588">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="cd825-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-589">Boolean</span></span>|<span data-ttu-id="cd825-590">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="cd825-590">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="cd825-591">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="cd825-591">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="cd825-592">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-592">Boolean</span></span>|<span data-ttu-id="cd825-593">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="cd825-593">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="cd825-594">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="cd825-594">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="cd825-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-595">Boolean</span></span>|<span data-ttu-id="cd825-596">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="cd825-596">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="cd825-597">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="cd825-597">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="cd825-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-598">Boolean</span></span>|<span data-ttu-id="cd825-599">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="cd825-599">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="cd825-600">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="cd825-600">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="cd825-601">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="cd825-601">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="cd825-602">指定聚焦的类型。</span><span class="sxs-lookup"><span data-stu-id="cd825-602">Specifies the type of Spotlight.</span></span> <span data-ttu-id="cd825-603">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="cd825-603">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="cd825-604">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="cd825-604">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="cd825-605">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-605">Boolean</span></span>|<span data-ttu-id="cd825-606">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="cd825-606">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="cd825-607">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="cd825-607">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="cd825-608">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="cd825-608">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="cd825-609">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-609">Boolean</span></span>|<span data-ttu-id="cd825-610">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="cd825-610">Disable automatic detection of settings.</span></span> <span data-ttu-id="cd825-611">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="cd825-611">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="cd825-612">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="cd825-612">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="cd825-613">String</span><span class="sxs-lookup"><span data-stu-id="cd825-613">String</span></span>|<span data-ttu-id="cd825-614">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="cd825-614">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="cd825-615">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="cd825-615">networkProxyServer</span></span>|[<span data-ttu-id="cd825-616">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="cd825-616">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="cd825-617">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="cd825-617">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="cd825-618">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="cd825-618">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="cd825-619">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-619">Boolean</span></span>|<span data-ttu-id="cd825-620">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="cd825-620">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="cd825-621">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-621">antiTheftModeBlocked</span></span>|<span data-ttu-id="cd825-622">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-622">Boolean</span></span>|<span data-ttu-id="cd825-623">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="cd825-623">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="cd825-624">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-624">bluetoothBlocked</span></span>|<span data-ttu-id="cd825-625">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-625">Boolean</span></span>|<span data-ttu-id="cd825-626">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="cd825-626">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="cd825-627">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-627">cameraBlocked</span></span>|<span data-ttu-id="cd825-628">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-628">Boolean</span></span>|<span data-ttu-id="cd825-629">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="cd825-629">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="cd825-630">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-630">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="cd825-631">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-631">Boolean</span></span>|<span data-ttu-id="cd825-632">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="cd825-632">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="cd825-633">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="cd825-633">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="cd825-634">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-634">Boolean</span></span>|<span data-ttu-id="cd825-635">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="cd825-635">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="cd825-636">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-636">copyPasteBlocked</span></span>|<span data-ttu-id="cd825-637">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-637">Boolean</span></span>|<span data-ttu-id="cd825-638">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="cd825-638">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="cd825-639">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-639">cortanaBlocked</span></span>|<span data-ttu-id="cd825-640">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-640">Boolean</span></span>|<span data-ttu-id="cd825-641">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="cd825-641">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="cd825-642">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="cd825-642">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="cd825-643">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-643">Boolean</span></span>|<span data-ttu-id="cd825-644">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="cd825-644">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="cd825-645">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="cd825-645">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="cd825-646">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-646">Boolean</span></span>|<span data-ttu-id="cd825-647">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="cd825-647">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="cd825-648">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="cd825-648">safeSearchFilter</span></span>|[<span data-ttu-id="cd825-649">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="cd825-649">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="cd825-650">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="cd825-650">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="cd825-651">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="cd825-651">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="cd825-652">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="cd825-652">edgeBlockPopups</span></span>|<span data-ttu-id="cd825-653">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-653">Boolean</span></span>|<span data-ttu-id="cd825-654">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="cd825-654">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="cd825-655">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="cd825-655">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="cd825-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-656">Boolean</span></span>|<span data-ttu-id="cd825-657">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="cd825-657">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="cd825-658">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="cd825-658">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="cd825-659">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-659">Boolean</span></span>|<span data-ttu-id="cd825-660">指示是否将 Intranet 流量从 Edge 切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="cd825-660">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="cd825-661">注意：此属性的名称令人误解;属性已过时，请改为使用 EdgeSendIntranetTrafficToInternetExplorer。</span><span class="sxs-lookup"><span data-stu-id="cd825-661">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="cd825-662">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="cd825-662">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="cd825-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-663">Boolean</span></span>|<span data-ttu-id="cd825-664">指示是否将 Intranet 流量从 Edge 切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="cd825-664">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="cd825-665">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="cd825-665">edgeRequireSmartScreen</span></span>|<span data-ttu-id="cd825-666">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-666">Boolean</span></span>|<span data-ttu-id="cd825-667">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="cd825-667">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="cd825-668">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="cd825-668">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="cd825-669">String</span><span class="sxs-lookup"><span data-stu-id="cd825-669">String</span></span>|<span data-ttu-id="cd825-670">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="cd825-670">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="cd825-671">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="cd825-671">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="cd825-672">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="cd825-672">edgeFirstRunUrl</span></span>|<span data-ttu-id="cd825-673">String</span><span class="sxs-lookup"><span data-stu-id="cd825-673">String</span></span>|<span data-ttu-id="cd825-674">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="cd825-674">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="cd825-675">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="cd825-675">edgeSearchEngine</span></span>|[<span data-ttu-id="cd825-676">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="cd825-676">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="cd825-677">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="cd825-677">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="cd825-678">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="cd825-678">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="cd825-679">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="cd825-679">edgeHomepageUrls</span></span>|<span data-ttu-id="cd825-680">String 集合</span><span class="sxs-lookup"><span data-stu-id="cd825-680">String collection</span></span>|<span data-ttu-id="cd825-681">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="cd825-681">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="cd825-682">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="cd825-682">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="cd825-683">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-683">Boolean</span></span>|<span data-ttu-id="cd825-684">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="cd825-684">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="cd825-685">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="cd825-685">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="cd825-686">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-686">Boolean</span></span>|<span data-ttu-id="cd825-687">指示用户是否可以替代有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="cd825-687">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="cd825-688">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="cd825-688">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="cd825-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-689">Boolean</span></span>|<span data-ttu-id="cd825-690">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="cd825-690">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="cd825-691">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="cd825-691">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="cd825-692">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-692">Boolean</span></span>|<span data-ttu-id="cd825-693">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="cd825-693">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="cd825-694">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-694">internetSharingBlocked</span></span>|<span data-ttu-id="cd825-695">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-695">Boolean</span></span>|<span data-ttu-id="cd825-696">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="cd825-696">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="cd825-697">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="cd825-697">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="cd825-698">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-698">Boolean</span></span>|<span data-ttu-id="cd825-699">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="cd825-699">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="cd825-700">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="cd825-700">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="cd825-701">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-701">Boolean</span></span>|<span data-ttu-id="cd825-702">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="cd825-702">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="cd825-703">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="cd825-703">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="cd825-704">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-704">Boolean</span></span>|<span data-ttu-id="cd825-705">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="cd825-705">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="cd825-706">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="cd825-706">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="cd825-707">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-707">Boolean</span></span>|<span data-ttu-id="cd825-708">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="cd825-708">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="cd825-709">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="cd825-709">settingsBlockChangeRegion</span></span>|<span data-ttu-id="cd825-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-710">Boolean</span></span>|<span data-ttu-id="cd825-711">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="cd825-711">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="cd825-712">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="cd825-712">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="cd825-713">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-713">Boolean</span></span>|<span data-ttu-id="cd825-714">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="cd825-714">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="cd825-715">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="cd825-715">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="cd825-716">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-716">Boolean</span></span>|<span data-ttu-id="cd825-717">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="cd825-717">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="cd825-718">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-718">locationServicesBlocked</span></span>|<span data-ttu-id="cd825-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-719">Boolean</span></span>|<span data-ttu-id="cd825-720">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="cd825-720">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="cd825-721">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-721">microsoftAccountBlocked</span></span>|<span data-ttu-id="cd825-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-722">Boolean</span></span>|<span data-ttu-id="cd825-723">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="cd825-723">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="cd825-724">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="cd825-724">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="cd825-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-725">Boolean</span></span>|<span data-ttu-id="cd825-726">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="cd825-726">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="cd825-727">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-727">nfcBlocked</span></span>|<span data-ttu-id="cd825-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-728">Boolean</span></span>|<span data-ttu-id="cd825-729">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="cd825-729">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="cd825-730">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-730">resetProtectionModeBlocked</span></span>|<span data-ttu-id="cd825-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-731">Boolean</span></span>|<span data-ttu-id="cd825-732">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="cd825-732">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="cd825-733">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-733">screenCaptureBlocked</span></span>|<span data-ttu-id="cd825-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-734">Boolean</span></span>|<span data-ttu-id="cd825-735">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="cd825-735">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="cd825-736">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="cd825-736">storageBlockRemovableStorage</span></span>|<span data-ttu-id="cd825-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-737">Boolean</span></span>|<span data-ttu-id="cd825-738">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="cd825-738">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="cd825-739">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="cd825-739">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="cd825-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-740">Boolean</span></span>|<span data-ttu-id="cd825-741">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="cd825-741">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="cd825-742">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-742">usbBlocked</span></span>|<span data-ttu-id="cd825-743">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-743">Boolean</span></span>|<span data-ttu-id="cd825-744">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="cd825-744">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="cd825-745">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-745">voiceRecordingBlocked</span></span>|<span data-ttu-id="cd825-746">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-746">Boolean</span></span>|<span data-ttu-id="cd825-747">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="cd825-747">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="cd825-748">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="cd825-748">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="cd825-749">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-749">Boolean</span></span>|<span data-ttu-id="cd825-750">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="cd825-750">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="cd825-751">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="cd825-751">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="cd825-752">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-752">wiFiBlocked</span></span>|<span data-ttu-id="cd825-753">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-753">Boolean</span></span>|<span data-ttu-id="cd825-754">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="cd825-754">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="cd825-755">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd825-755">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="cd825-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-756">Boolean</span></span>|<span data-ttu-id="cd825-757">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="cd825-757">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="cd825-758">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="cd825-758">wiFiScanInterval</span></span>|<span data-ttu-id="cd825-759">Int32</span><span class="sxs-lookup"><span data-stu-id="cd825-759">Int32</span></span>|<span data-ttu-id="cd825-760">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="cd825-760">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="cd825-761">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="cd825-761">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="cd825-762">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="cd825-762">Valid values 1 to 500</span></span>|
|<span data-ttu-id="cd825-763">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="cd825-763">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="cd825-764">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-764">Boolean</span></span>|<span data-ttu-id="cd825-765">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="cd825-765">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="cd825-766">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="cd825-766">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="cd825-767">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-767">Boolean</span></span>|<span data-ttu-id="cd825-768">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="cd825-768">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="cd825-769">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="cd825-769">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="cd825-770">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-770">Boolean</span></span>|<span data-ttu-id="cd825-771">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="cd825-771">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="cd825-772">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-772">windowsStoreBlocked</span></span>|<span data-ttu-id="cd825-773">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-773">Boolean</span></span>|<span data-ttu-id="cd825-774">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="cd825-774">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="cd825-775">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="cd825-775">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="cd825-776">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="cd825-776">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="cd825-777">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="cd825-777">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="cd825-778">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="cd825-778">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="cd825-779">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="cd825-779">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="cd825-780">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-780">Boolean</span></span>|<span data-ttu-id="cd825-781">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="cd825-781">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="cd825-782">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="cd825-782">developerUnlockSetting</span></span>|[<span data-ttu-id="cd825-783">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="cd825-783">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="cd825-784">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="cd825-784">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="cd825-785">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="cd825-785">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="cd825-786">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="cd825-786">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="cd825-787">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-787">Boolean</span></span>|<span data-ttu-id="cd825-788">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="cd825-788">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="cd825-789">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="cd825-789">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="cd825-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-790">Boolean</span></span>|<span data-ttu-id="cd825-791">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="cd825-791">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="cd825-792">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="cd825-792">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="cd825-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-793">Boolean</span></span>|<span data-ttu-id="cd825-794">指示是否启用“仅限专用应用商店”。</span><span class="sxs-lookup"><span data-stu-id="cd825-794">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="cd825-795">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="cd825-795">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="cd825-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-796">Boolean</span></span>|<span data-ttu-id="cd825-797">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="cd825-797">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="cd825-798">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="cd825-798">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="cd825-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-799">Boolean</span></span>|<span data-ttu-id="cd825-800">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="cd825-800">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="cd825-801">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="cd825-801">gameDvrBlocked</span></span>|<span data-ttu-id="cd825-802">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-802">Boolean</span></span>|<span data-ttu-id="cd825-803">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="cd825-803">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="cd825-804">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="cd825-804">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="cd825-805">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-805">Boolean</span></span>|<span data-ttu-id="cd825-806">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="cd825-806">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="cd825-807">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="cd825-807">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="cd825-808">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-808">Boolean</span></span>|<span data-ttu-id="cd825-809">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="cd825-809">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="cd825-810">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="cd825-810">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="cd825-811">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-811">Boolean</span></span>|<span data-ttu-id="cd825-812">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="cd825-812">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="cd825-813">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="cd825-813">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="cd825-814">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-814">Boolean</span></span>|<span data-ttu-id="cd825-815">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="cd825-815">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="cd825-816">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="cd825-816">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="cd825-817">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd825-817">Boolean</span></span>|<span data-ttu-id="cd825-818">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="cd825-818">Whether the device is required to connect to the network.</span></span>|



## <a name="response"></a><span data-ttu-id="cd825-819">响应</span><span class="sxs-lookup"><span data-stu-id="cd825-819">Response</span></span>
<span data-ttu-id="cd825-820">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd825-820">If successful, this method returns a `201 Created` response code and a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd825-821">示例</span><span class="sxs-lookup"><span data-stu-id="cd825-821">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd825-822">请求</span><span class="sxs-lookup"><span data-stu-id="cd825-822">Request</span></span>
<span data-ttu-id="cd825-823">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd825-823">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 9822

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderScanDownloads": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderMonitorFileActivity": "disable",
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderScanMaxCpu": 2,
  "defenderScanArchiveFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderRequireCloudProtection": true,
  "defenderCloudBlockLevel": "high",
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScanType": "disabled",
  "defenderSystemScanSchedule": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```

### <a name="response"></a><span data-ttu-id="cd825-824">响应</span><span class="sxs-lookup"><span data-stu-id="cd825-824">Response</span></span>
<span data-ttu-id="cd825-p159">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd825-p159">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9994

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderScanDownloads": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderMonitorFileActivity": "disable",
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderScanMaxCpu": 2,
  "defenderScanArchiveFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderRequireCloudProtection": true,
  "defenderCloudBlockLevel": "high",
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScanType": "disabled",
  "defenderSystemScanSchedule": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```




