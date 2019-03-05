---
title: 创建 windows10GeneralConfiguration
description: 创建新的 windows10GeneralConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2ce4b861ca6825af4046edc0fd13322d4d763ac
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255984"
---
# <a name="create-windows10generalconfiguration"></a><span data-ttu-id="85504-103">创建 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="85504-103">Create windows10GeneralConfiguration</span></span>

> <span data-ttu-id="85504-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85504-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85504-105">创建新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85504-105">Create a new [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85504-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="85504-106">Prerequisites</span></span>
<span data-ttu-id="85504-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="85504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="85504-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="85504-109">Permission type</span></span>|<span data-ttu-id="85504-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85504-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85504-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85504-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85504-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85504-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85504-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85504-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85504-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="85504-114">Not supported.</span></span>|
|<span data-ttu-id="85504-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="85504-115">Application</span></span>|<span data-ttu-id="85504-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="85504-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85504-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85504-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="85504-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="85504-118">Request headers</span></span>
|<span data-ttu-id="85504-119">标头</span><span class="sxs-lookup"><span data-stu-id="85504-119">Header</span></span>|<span data-ttu-id="85504-120">值</span><span class="sxs-lookup"><span data-stu-id="85504-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85504-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="85504-121">Authorization</span></span>|<span data-ttu-id="85504-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85504-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85504-123">Accept</span><span class="sxs-lookup"><span data-stu-id="85504-123">Accept</span></span>|<span data-ttu-id="85504-124">application/json</span><span class="sxs-lookup"><span data-stu-id="85504-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85504-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="85504-125">Request body</span></span>
<span data-ttu-id="85504-126">在请求正文中，提供 windows10GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85504-126">In the request body, supply a JSON representation for the windows10GeneralConfiguration object.</span></span>

<span data-ttu-id="85504-127">下表显示了创建 windows10GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="85504-127">The following table shows the properties that are required when you create the windows10GeneralConfiguration.</span></span>

|<span data-ttu-id="85504-128">属性</span><span class="sxs-lookup"><span data-stu-id="85504-128">Property</span></span>|<span data-ttu-id="85504-129">类型</span><span class="sxs-lookup"><span data-stu-id="85504-129">Type</span></span>|<span data-ttu-id="85504-130">说明</span><span class="sxs-lookup"><span data-stu-id="85504-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85504-131">id</span><span class="sxs-lookup"><span data-stu-id="85504-131">id</span></span>|<span data-ttu-id="85504-132">字符串</span><span class="sxs-lookup"><span data-stu-id="85504-132">String</span></span>|<span data-ttu-id="85504-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="85504-133">Key of the entity.</span></span> <span data-ttu-id="85504-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85504-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85504-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85504-135">lastModifiedDateTime</span></span>|<span data-ttu-id="85504-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85504-136">DateTimeOffset</span></span>|<span data-ttu-id="85504-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="85504-137">DateTime the object was last modified.</span></span> <span data-ttu-id="85504-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85504-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85504-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85504-139">createdDateTime</span></span>|<span data-ttu-id="85504-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85504-140">DateTimeOffset</span></span>|<span data-ttu-id="85504-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="85504-141">DateTime the object was created.</span></span> <span data-ttu-id="85504-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85504-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85504-143">description</span><span class="sxs-lookup"><span data-stu-id="85504-143">description</span></span>|<span data-ttu-id="85504-144">字符串</span><span class="sxs-lookup"><span data-stu-id="85504-144">String</span></span>|<span data-ttu-id="85504-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="85504-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="85504-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85504-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85504-147">displayName</span><span class="sxs-lookup"><span data-stu-id="85504-147">displayName</span></span>|<span data-ttu-id="85504-148">String</span><span class="sxs-lookup"><span data-stu-id="85504-148">String</span></span>|<span data-ttu-id="85504-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="85504-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="85504-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85504-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85504-151">version</span><span class="sxs-lookup"><span data-stu-id="85504-151">version</span></span>|<span data-ttu-id="85504-152">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-152">Int32</span></span>|<span data-ttu-id="85504-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="85504-153">Version of the device configuration.</span></span> <span data-ttu-id="85504-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85504-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85504-155">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="85504-155">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="85504-156">String</span><span class="sxs-lookup"><span data-stu-id="85504-156">String</span></span>|<span data-ttu-id="85504-157">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="85504-157">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="85504-158">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="85504-158">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="85504-159">String</span><span class="sxs-lookup"><span data-stu-id="85504-159">String</span></span>|<span data-ttu-id="85504-160">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="85504-160">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="85504-161">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="85504-161">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="85504-162">String</span><span class="sxs-lookup"><span data-stu-id="85504-162">String</span></span>|<span data-ttu-id="85504-163">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="85504-163">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="85504-164">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="85504-164">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="85504-165">String</span><span class="sxs-lookup"><span data-stu-id="85504-165">String</span></span>|<span data-ttu-id="85504-166">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="85504-166">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="85504-167">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="85504-167">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="85504-168">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-168">Int32</span></span>|<span data-ttu-id="85504-169">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="85504-169">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="85504-170">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="85504-170">This is a mobile only setting.</span></span> <span data-ttu-id="85504-171">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="85504-171">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="85504-172">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="85504-172">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="85504-173">String</span><span class="sxs-lookup"><span data-stu-id="85504-173">String</span></span>|<span data-ttu-id="85504-174">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="85504-174">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="85504-175">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="85504-175">searchBlockDiacritics</span></span>|<span data-ttu-id="85504-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-176">Boolean</span></span>|<span data-ttu-id="85504-177">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="85504-177">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="85504-178">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="85504-178">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="85504-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-179">Boolean</span></span>|<span data-ttu-id="85504-180">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="85504-180">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="85504-181">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="85504-181">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="85504-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-182">Boolean</span></span>|<span data-ttu-id="85504-183">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="85504-183">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="85504-184">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="85504-184">searchEnableRemoteQueries</span></span>|<span data-ttu-id="85504-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-185">Boolean</span></span>|<span data-ttu-id="85504-186">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="85504-186">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="85504-187">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="85504-187">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="85504-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-188">Boolean</span></span>|<span data-ttu-id="85504-189">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="85504-189">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="85504-190">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="85504-190">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="85504-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-191">Boolean</span></span>|<span data-ttu-id="85504-192">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="85504-192">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="85504-193">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="85504-193">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="85504-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-194">Boolean</span></span>|<span data-ttu-id="85504-195">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="85504-195">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="85504-196">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="85504-196">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="85504-197">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="85504-197">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="85504-198">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="85504-198">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="85504-199">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="85504-199">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="85504-200">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="85504-200">oneDriveDisableFileSync</span></span>|<span data-ttu-id="85504-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-201">Boolean</span></span>|<span data-ttu-id="85504-202">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="85504-202">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="85504-203">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="85504-203">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="85504-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-204">Boolean</span></span>|<span data-ttu-id="85504-205">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="85504-205">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="85504-206">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="85504-206">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="85504-207">String</span><span class="sxs-lookup"><span data-stu-id="85504-207">String</span></span>|<span data-ttu-id="85504-208">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="85504-208">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="85504-209">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="85504-209">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="85504-210">String</span><span class="sxs-lookup"><span data-stu-id="85504-210">String</span></span>|<span data-ttu-id="85504-211">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="85504-211">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="85504-212">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="85504-212">bluetoothAllowedServices</span></span>|<span data-ttu-id="85504-213">String collection</span><span class="sxs-lookup"><span data-stu-id="85504-213">String collection</span></span>|<span data-ttu-id="85504-214">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="85504-214">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="85504-215">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="85504-215">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="85504-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-216">Boolean</span></span>|<span data-ttu-id="85504-217">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="85504-217">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="85504-218">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="85504-218">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="85504-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-219">Boolean</span></span>|<span data-ttu-id="85504-220">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="85504-220">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="85504-221">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="85504-221">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="85504-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-222">Boolean</span></span>|<span data-ttu-id="85504-223">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="85504-223">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="85504-224">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="85504-224">edgeBlockAutofill</span></span>|<span data-ttu-id="85504-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-225">Boolean</span></span>|<span data-ttu-id="85504-226">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="85504-226">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="85504-227">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-227">edgeBlocked</span></span>|<span data-ttu-id="85504-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-228">Boolean</span></span>|<span data-ttu-id="85504-229">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="85504-229">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="85504-230">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="85504-230">edgeCookiePolicy</span></span>|[<span data-ttu-id="85504-231">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="85504-231">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="85504-232">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="85504-232">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="85504-233">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="85504-233">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="85504-234">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="85504-234">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="85504-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-235">Boolean</span></span>|<span data-ttu-id="85504-236">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="85504-236">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="85504-237">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="85504-237">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="85504-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-238">Boolean</span></span>|<span data-ttu-id="85504-239">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="85504-239">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="85504-240">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="85504-240">edgeBlockExtensions</span></span>|<span data-ttu-id="85504-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-241">Boolean</span></span>|<span data-ttu-id="85504-242">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="85504-242">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="85504-243">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="85504-243">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="85504-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-244">Boolean</span></span>|<span data-ttu-id="85504-245">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="85504-245">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="85504-246">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="85504-246">edgeBlockJavaScript</span></span>|<span data-ttu-id="85504-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-247">Boolean</span></span>|<span data-ttu-id="85504-248">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="85504-248">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="85504-249">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="85504-249">edgeBlockPasswordManager</span></span>|<span data-ttu-id="85504-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-250">Boolean</span></span>|<span data-ttu-id="85504-251">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="85504-251">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="85504-252">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="85504-252">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="85504-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-253">Boolean</span></span>|<span data-ttu-id="85504-254">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="85504-254">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="85504-255">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="85504-255">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="85504-256">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="85504-256">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="85504-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-257">Boolean</span></span>|<span data-ttu-id="85504-258">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="85504-258">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="85504-259">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="85504-259">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="85504-260">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="85504-260">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="85504-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-261">Boolean</span></span>|<span data-ttu-id="85504-262">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="85504-262">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="85504-263">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="85504-263">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="85504-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-264">Boolean</span></span>|<span data-ttu-id="85504-265">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="85504-265">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="85504-266">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="85504-266">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="85504-267">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="85504-267">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="85504-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-268">Boolean</span></span>|<span data-ttu-id="85504-269">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="85504-269">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="85504-270">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="85504-270">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="85504-271">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="85504-271">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="85504-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-272">Boolean</span></span>|<span data-ttu-id="85504-273">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="85504-273">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="85504-274">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="85504-274">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="85504-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-275">Boolean</span></span>|<span data-ttu-id="85504-276">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="85504-276">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="85504-277">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="85504-277">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="85504-278">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="85504-278">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="85504-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-279">Boolean</span></span>|<span data-ttu-id="85504-280">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="85504-280">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="85504-281">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="85504-281">cellularBlockVpn</span></span>|<span data-ttu-id="85504-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-282">Boolean</span></span>|<span data-ttu-id="85504-283">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="85504-283">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="85504-284">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="85504-284">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="85504-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-285">Boolean</span></span>|<span data-ttu-id="85504-286">是否阻止用户在通过手机网络漫游时使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="85504-286">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="85504-287">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="85504-287">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="85504-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-288">Boolean</span></span>|<span data-ttu-id="85504-289">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="85504-289">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="85504-290">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="85504-290">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="85504-291">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-291">Int32</span></span>|<span data-ttu-id="85504-292">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="85504-292">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="85504-293">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="85504-293">Valid values 0 to 90</span></span>|
|<span data-ttu-id="85504-294">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="85504-294">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="85504-295">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="85504-295">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="85504-296">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="85504-296">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="85504-297">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="85504-297">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="85504-298">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="85504-298">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="85504-299">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="85504-299">Defender day of the week for the system scan.</span></span> <span data-ttu-id="85504-300">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="85504-300">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="85504-301">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="85504-301">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="85504-302">String 集合</span><span class="sxs-lookup"><span data-stu-id="85504-302">String collection</span></span>|<span data-ttu-id="85504-303">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="85504-303">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="85504-304">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="85504-304">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="85504-305">String collection</span><span class="sxs-lookup"><span data-stu-id="85504-305">String collection</span></span>|<span data-ttu-id="85504-306">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="85504-306">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="85504-307">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="85504-307">defenderScanMaxCpu</span></span>|<span data-ttu-id="85504-308">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-308">Int32</span></span>|<span data-ttu-id="85504-309">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="85504-309">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="85504-310">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="85504-310">Valid values 0 to 100</span></span>|
|<span data-ttu-id="85504-311">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="85504-311">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="85504-312">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="85504-312">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="85504-313">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="85504-313">Value for monitoring file activity.</span></span> <span data-ttu-id="85504-314">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="85504-314">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="85504-315">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="85504-315">defenderProcessesToExclude</span></span>|<span data-ttu-id="85504-316">String 集合</span><span class="sxs-lookup"><span data-stu-id="85504-316">String collection</span></span>|<span data-ttu-id="85504-317">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="85504-317">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="85504-318">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="85504-318">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="85504-319">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="85504-319">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="85504-320">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="85504-320">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="85504-321">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="85504-321">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="85504-322">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="85504-322">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="85504-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-323">Boolean</span></span>|<span data-ttu-id="85504-324">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="85504-324">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="85504-325">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="85504-325">defenderRequireCloudProtection</span></span>|<span data-ttu-id="85504-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-326">Boolean</span></span>|<span data-ttu-id="85504-327">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="85504-327">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="85504-328">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="85504-328">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="85504-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-329">Boolean</span></span>|<span data-ttu-id="85504-330">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="85504-330">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="85504-331">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="85504-331">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="85504-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-332">Boolean</span></span>|<span data-ttu-id="85504-333">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="85504-333">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="85504-334">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="85504-334">defenderScanArchiveFiles</span></span>|<span data-ttu-id="85504-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-335">Boolean</span></span>|<span data-ttu-id="85504-336">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="85504-336">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="85504-337">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="85504-337">defenderScanDownloads</span></span>|<span data-ttu-id="85504-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-338">Boolean</span></span>|<span data-ttu-id="85504-339">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="85504-339">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="85504-340">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="85504-340">defenderScanNetworkFiles</span></span>|<span data-ttu-id="85504-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-341">Boolean</span></span>|<span data-ttu-id="85504-342">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="85504-342">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="85504-343">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="85504-343">defenderScanIncomingMail</span></span>|<span data-ttu-id="85504-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-344">Boolean</span></span>|<span data-ttu-id="85504-345">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="85504-345">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="85504-346">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="85504-346">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="85504-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-347">Boolean</span></span>|<span data-ttu-id="85504-348">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="85504-348">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="85504-349">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="85504-349">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="85504-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-350">Boolean</span></span>|<span data-ttu-id="85504-351">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="85504-351">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="85504-352">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="85504-352">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="85504-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-353">Boolean</span></span>|<span data-ttu-id="85504-354">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="85504-354">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="85504-355">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="85504-355">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="85504-356">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-356">Int32</span></span>|<span data-ttu-id="85504-357">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="85504-357">The signature update interval in hours.</span></span> <span data-ttu-id="85504-358">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="85504-358">Specify 0 not to check.</span></span> <span data-ttu-id="85504-359">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="85504-359">Valid values 0 to 24</span></span>|
|<span data-ttu-id="85504-360">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="85504-360">defenderScanType</span></span>|[<span data-ttu-id="85504-361">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="85504-361">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="85504-362">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="85504-362">The defender system scan type.</span></span> <span data-ttu-id="85504-363">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="85504-363">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="85504-364">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="85504-364">defenderScheduledScanTime</span></span>|<span data-ttu-id="85504-365">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="85504-365">TimeOfDay</span></span>|<span data-ttu-id="85504-366">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="85504-366">The defender time for the system scan.</span></span>|
|<span data-ttu-id="85504-367">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="85504-367">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="85504-368">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="85504-368">TimeOfDay</span></span>|<span data-ttu-id="85504-369">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="85504-369">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="85504-370">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="85504-370">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="85504-371">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="85504-371">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="85504-372">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="85504-372">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="85504-373">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="85504-373">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="85504-374">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="85504-374">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="85504-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-375">Boolean</span></span>|<span data-ttu-id="85504-376">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="85504-376">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="85504-377">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="85504-377">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="85504-378">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="85504-378">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="85504-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-379">Boolean</span></span>|<span data-ttu-id="85504-380">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="85504-380">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="85504-381">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="85504-381">lockScreenBlockCortana</span></span>|<span data-ttu-id="85504-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-382">Boolean</span></span>|<span data-ttu-id="85504-383">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="85504-383">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="85504-384">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="85504-384">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="85504-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-385">Boolean</span></span>|<span data-ttu-id="85504-386">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="85504-386">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="85504-387">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="85504-387">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="85504-388">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-388">Int32</span></span>|<span data-ttu-id="85504-389">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="85504-389">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="85504-390">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="85504-390">Supported values are 11-1800.</span></span> <span data-ttu-id="85504-391">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="85504-391">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="85504-392">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="85504-392">passwordBlockSimple</span></span>|<span data-ttu-id="85504-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-393">Boolean</span></span>|<span data-ttu-id="85504-394">指定是否允许 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="85504-394">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="85504-395">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="85504-395">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="85504-396">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="85504-396">passwordExpirationDays</span></span>|<span data-ttu-id="85504-397">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-397">Int32</span></span>|<span data-ttu-id="85504-398">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="85504-398">The password expiration in days.</span></span> <span data-ttu-id="85504-399">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="85504-399">Valid values 0 to 730</span></span>|
|<span data-ttu-id="85504-400">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="85504-400">passwordMinimumLength</span></span>|<span data-ttu-id="85504-401">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-401">Int32</span></span>|<span data-ttu-id="85504-402">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="85504-402">The minimum password length.</span></span> <span data-ttu-id="85504-403">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="85504-403">Valid values 4 to 16</span></span>|
|<span data-ttu-id="85504-404">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="85504-404">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="85504-405">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-405">Int32</span></span>|<span data-ttu-id="85504-406">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="85504-406">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="85504-407">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="85504-407">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="85504-408">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-408">Int32</span></span>|<span data-ttu-id="85504-409">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="85504-409">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="85504-410">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="85504-410">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="85504-411">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-411">Int32</span></span>|<span data-ttu-id="85504-412">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="85504-412">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="85504-413">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="85504-413">Valid values 0 to 50</span></span>|
|<span data-ttu-id="85504-414">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="85504-414">passwordRequired</span></span>|<span data-ttu-id="85504-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-415">Boolean</span></span>|<span data-ttu-id="85504-416">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="85504-416">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="85504-417">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="85504-417">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="85504-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-418">Boolean</span></span>|<span data-ttu-id="85504-419">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="85504-419">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="85504-420">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="85504-420">passwordRequiredType</span></span>|[<span data-ttu-id="85504-421">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="85504-421">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="85504-422">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="85504-422">The required password type.</span></span> <span data-ttu-id="85504-423">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="85504-423">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="85504-424">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="85504-424">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="85504-425">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-425">Int32</span></span>|<span data-ttu-id="85504-426">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="85504-426">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="85504-427">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="85504-427">Valid values 0 to 999</span></span>|
|<span data-ttu-id="85504-428">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="85504-428">privacyAdvertisingId</span></span>|[<span data-ttu-id="85504-429">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="85504-429">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="85504-430">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="85504-430">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="85504-431">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="85504-431">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="85504-432">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="85504-432">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="85504-433">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="85504-433">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="85504-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-434">Boolean</span></span>|<span data-ttu-id="85504-435">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="85504-435">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="85504-436">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="85504-436">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="85504-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-437">Boolean</span></span>|<span data-ttu-id="85504-438">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="85504-438">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="85504-439">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="85504-439">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="85504-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-440">Boolean</span></span>|<span data-ttu-id="85504-441">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="85504-441">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="85504-442">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="85504-442">startMenuAppListVisibility</span></span>|[<span data-ttu-id="85504-443">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="85504-443">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="85504-444">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="85504-444">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="85504-445">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="85504-445">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="85504-446">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="85504-446">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="85504-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-447">Boolean</span></span>|<span data-ttu-id="85504-448">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="85504-448">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="85504-449">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="85504-449">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="85504-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-450">Boolean</span></span>|<span data-ttu-id="85504-451">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="85504-451">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="85504-452">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="85504-452">startMenuHideHibernate</span></span>|<span data-ttu-id="85504-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-453">Boolean</span></span>|<span data-ttu-id="85504-454">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="85504-454">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="85504-455">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="85504-455">startMenuHideLock</span></span>|<span data-ttu-id="85504-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-456">Boolean</span></span>|<span data-ttu-id="85504-457">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="85504-457">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="85504-458">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="85504-458">startMenuHidePowerButton</span></span>|<span data-ttu-id="85504-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-459">Boolean</span></span>|<span data-ttu-id="85504-460">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="85504-460">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="85504-461">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="85504-461">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="85504-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-462">Boolean</span></span>|<span data-ttu-id="85504-463">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="85504-463">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="85504-464">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="85504-464">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="85504-465">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-465">Boolean</span></span>|<span data-ttu-id="85504-466">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="85504-466">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="85504-467">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="85504-467">startMenuHideRestartOptions</span></span>|<span data-ttu-id="85504-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-468">Boolean</span></span>|<span data-ttu-id="85504-469">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="85504-469">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="85504-470">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="85504-470">startMenuHideShutDown</span></span>|<span data-ttu-id="85504-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-471">Boolean</span></span>|<span data-ttu-id="85504-472">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="85504-472">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="85504-473">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="85504-473">startMenuHideSignOut</span></span>|<span data-ttu-id="85504-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-474">Boolean</span></span>|<span data-ttu-id="85504-475">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="85504-475">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="85504-476">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="85504-476">startMenuHideSleep</span></span>|<span data-ttu-id="85504-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-477">Boolean</span></span>|<span data-ttu-id="85504-478">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="85504-478">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="85504-479">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="85504-479">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="85504-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-480">Boolean</span></span>|<span data-ttu-id="85504-481">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="85504-481">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="85504-482">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="85504-482">startMenuHideUserTile</span></span>|<span data-ttu-id="85504-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-483">Boolean</span></span>|<span data-ttu-id="85504-484">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="85504-484">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="85504-485">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="85504-485">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="85504-486">Binary</span><span class="sxs-lookup"><span data-stu-id="85504-486">Binary</span></span>|<span data-ttu-id="85504-487">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="85504-487">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="85504-488">开始布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="85504-488">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="85504-489">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="85504-489">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="85504-490">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="85504-490">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="85504-491">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="85504-491">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="85504-492">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="85504-492">startMenuLayoutXml</span></span>|<span data-ttu-id="85504-493">Binary</span><span class="sxs-lookup"><span data-stu-id="85504-493">Binary</span></span>|<span data-ttu-id="85504-494">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="85504-494">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="85504-495">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="85504-495">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="85504-496">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="85504-496">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="85504-497">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="85504-497">startMenuMode</span></span>|[<span data-ttu-id="85504-498">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="85504-498">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="85504-499">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="85504-499">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="85504-500">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="85504-500">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="85504-501">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="85504-501">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="85504-502">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="85504-502">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="85504-503">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="85504-503">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="85504-504">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="85504-504">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="85504-505">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="85504-505">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="85504-506">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="85504-506">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="85504-507">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="85504-507">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="85504-508">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="85504-508">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="85504-509">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="85504-509">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="85504-510">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="85504-510">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="85504-511">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="85504-511">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="85504-512">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="85504-512">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="85504-513">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="85504-513">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="85504-514">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="85504-514">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="85504-515">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="85504-515">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="85504-516">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="85504-516">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="85504-517">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="85504-517">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="85504-518">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="85504-518">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="85504-519">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="85504-519">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="85504-520">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="85504-520">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="85504-521">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="85504-521">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="85504-522">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="85504-522">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="85504-523">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="85504-523">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="85504-524">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="85504-524">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="85504-525">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="85504-525">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="85504-526">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="85504-526">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="85504-527">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="85504-527">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="85504-528">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="85504-528">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="85504-529">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="85504-529">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="85504-530">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="85504-530">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="85504-531">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="85504-531">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="85504-532">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="85504-532">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="85504-533">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="85504-533">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="85504-534">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="85504-534">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="85504-535">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="85504-535">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="85504-536">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="85504-536">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="85504-537">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="85504-537">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="85504-538">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="85504-538">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="85504-539">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="85504-539">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="85504-540">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="85504-540">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="85504-541">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="85504-541">settingsBlockSettingsApp</span></span>|<span data-ttu-id="85504-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-542">Boolean</span></span>|<span data-ttu-id="85504-543">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="85504-543">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="85504-544">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="85504-544">settingsBlockSystemPage</span></span>|<span data-ttu-id="85504-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-545">Boolean</span></span>|<span data-ttu-id="85504-546">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="85504-546">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="85504-547">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="85504-547">settingsBlockDevicesPage</span></span>|<span data-ttu-id="85504-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-548">Boolean</span></span>|<span data-ttu-id="85504-549">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="85504-549">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="85504-550">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="85504-550">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="85504-551">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-551">Boolean</span></span>|<span data-ttu-id="85504-552">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="85504-552">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="85504-553">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="85504-553">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="85504-554">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-554">Boolean</span></span>|<span data-ttu-id="85504-555">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="85504-555">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="85504-556">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="85504-556">settingsBlockAccountsPage</span></span>|<span data-ttu-id="85504-557">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-557">Boolean</span></span>|<span data-ttu-id="85504-558">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="85504-558">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="85504-559">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="85504-559">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="85504-560">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-560">Boolean</span></span>|<span data-ttu-id="85504-561">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="85504-561">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="85504-562">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="85504-562">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="85504-563">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-563">Boolean</span></span>|<span data-ttu-id="85504-564">指示是否阻止在“设置”应用中访问“辅助功能”。</span><span class="sxs-lookup"><span data-stu-id="85504-564">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="85504-565">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="85504-565">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="85504-566">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-566">Boolean</span></span>|<span data-ttu-id="85504-567">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="85504-567">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="85504-568">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="85504-568">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="85504-569">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-569">Boolean</span></span>|<span data-ttu-id="85504-570">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="85504-570">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="85504-571">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="85504-571">settingsBlockAppsPage</span></span>|<span data-ttu-id="85504-572">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-572">Boolean</span></span>|<span data-ttu-id="85504-573">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="85504-573">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="85504-574">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="85504-574">settingsBlockGamingPage</span></span>|<span data-ttu-id="85504-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-575">Boolean</span></span>|<span data-ttu-id="85504-576">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="85504-576">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="85504-577">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="85504-577">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="85504-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-578">Boolean</span></span>|<span data-ttu-id="85504-579">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="85504-579">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="85504-580">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-580">windowsSpotlightBlocked</span></span>|<span data-ttu-id="85504-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-581">Boolean</span></span>|<span data-ttu-id="85504-582">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="85504-582">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="85504-583">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="85504-583">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="85504-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-584">Boolean</span></span>|<span data-ttu-id="85504-585">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="85504-585">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="85504-586">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="85504-586">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="85504-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-587">Boolean</span></span>|<span data-ttu-id="85504-588">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="85504-588">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="85504-589">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="85504-589">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="85504-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-590">Boolean</span></span>|<span data-ttu-id="85504-591">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="85504-591">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="85504-592">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="85504-592">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="85504-593">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-593">Boolean</span></span>|<span data-ttu-id="85504-594">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="85504-594">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="85504-595">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="85504-595">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="85504-596">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-596">Boolean</span></span>|<span data-ttu-id="85504-597">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="85504-597">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="85504-598">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="85504-598">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="85504-599">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="85504-599">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="85504-600">指定聚光灯的类型。</span><span class="sxs-lookup"><span data-stu-id="85504-600">Specifies the type of Spotlight.</span></span> <span data-ttu-id="85504-601">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="85504-601">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="85504-602">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="85504-602">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="85504-603">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-603">Boolean</span></span>|<span data-ttu-id="85504-604">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="85504-604">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="85504-605">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="85504-605">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="85504-606">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="85504-606">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="85504-607">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-607">Boolean</span></span>|<span data-ttu-id="85504-608">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="85504-608">Disable automatic detection of settings.</span></span> <span data-ttu-id="85504-609">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="85504-609">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="85504-610">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="85504-610">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="85504-611">String</span><span class="sxs-lookup"><span data-stu-id="85504-611">String</span></span>|<span data-ttu-id="85504-612">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="85504-612">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="85504-613">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="85504-613">networkProxyServer</span></span>|[<span data-ttu-id="85504-614">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="85504-614">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="85504-615">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="85504-615">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="85504-616">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="85504-616">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="85504-617">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-617">Boolean</span></span>|<span data-ttu-id="85504-618">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="85504-618">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="85504-619">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-619">antiTheftModeBlocked</span></span>|<span data-ttu-id="85504-620">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-620">Boolean</span></span>|<span data-ttu-id="85504-621">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="85504-621">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="85504-622">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-622">bluetoothBlocked</span></span>|<span data-ttu-id="85504-623">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-623">Boolean</span></span>|<span data-ttu-id="85504-624">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="85504-624">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="85504-625">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-625">cameraBlocked</span></span>|<span data-ttu-id="85504-626">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-626">Boolean</span></span>|<span data-ttu-id="85504-627">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="85504-627">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="85504-628">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-628">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="85504-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-629">Boolean</span></span>|<span data-ttu-id="85504-630">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="85504-630">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="85504-631">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="85504-631">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="85504-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-632">Boolean</span></span>|<span data-ttu-id="85504-633">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="85504-633">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="85504-634">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-634">copyPasteBlocked</span></span>|<span data-ttu-id="85504-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-635">Boolean</span></span>|<span data-ttu-id="85504-636">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="85504-636">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="85504-637">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-637">cortanaBlocked</span></span>|<span data-ttu-id="85504-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-638">Boolean</span></span>|<span data-ttu-id="85504-639">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="85504-639">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="85504-640">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="85504-640">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="85504-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-641">Boolean</span></span>|<span data-ttu-id="85504-642">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="85504-642">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="85504-643">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="85504-643">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="85504-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-644">Boolean</span></span>|<span data-ttu-id="85504-645">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="85504-645">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="85504-646">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="85504-646">safeSearchFilter</span></span>|[<span data-ttu-id="85504-647">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="85504-647">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="85504-648">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="85504-648">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="85504-649">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="85504-649">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="85504-650">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="85504-650">edgeBlockPopups</span></span>|<span data-ttu-id="85504-651">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-651">Boolean</span></span>|<span data-ttu-id="85504-652">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="85504-652">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="85504-653">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="85504-653">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="85504-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-654">Boolean</span></span>|<span data-ttu-id="85504-655">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="85504-655">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="85504-656">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="85504-656">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="85504-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-657">Boolean</span></span>|<span data-ttu-id="85504-658">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="85504-658">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="85504-659">注意: 此属性的名称是误导性的;属性已过时, 请改用 EdgeSendIntranetTrafficToInternetExplorer。</span><span class="sxs-lookup"><span data-stu-id="85504-659">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="85504-660">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="85504-660">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="85504-661">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-661">Boolean</span></span>|<span data-ttu-id="85504-662">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="85504-662">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="85504-663">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="85504-663">edgeRequireSmartScreen</span></span>|<span data-ttu-id="85504-664">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-664">Boolean</span></span>|<span data-ttu-id="85504-665">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="85504-665">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="85504-666">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="85504-666">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="85504-667">String</span><span class="sxs-lookup"><span data-stu-id="85504-667">String</span></span>|<span data-ttu-id="85504-668">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="85504-668">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="85504-669">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="85504-669">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="85504-670">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="85504-670">edgeFirstRunUrl</span></span>|<span data-ttu-id="85504-671">String</span><span class="sxs-lookup"><span data-stu-id="85504-671">String</span></span>|<span data-ttu-id="85504-672">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="85504-672">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="85504-673">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="85504-673">edgeSearchEngine</span></span>|[<span data-ttu-id="85504-674">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="85504-674">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="85504-675">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="85504-675">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="85504-676">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="85504-676">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="85504-677">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="85504-677">edgeHomepageUrls</span></span>|<span data-ttu-id="85504-678">String 集合</span><span class="sxs-lookup"><span data-stu-id="85504-678">String collection</span></span>|<span data-ttu-id="85504-679">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="85504-679">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="85504-680">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="85504-680">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="85504-681">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-681">Boolean</span></span>|<span data-ttu-id="85504-682">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="85504-682">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="85504-683">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="85504-683">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="85504-684">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-684">Boolean</span></span>|<span data-ttu-id="85504-685">指示用户是否可以覆盖有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="85504-685">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="85504-686">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="85504-686">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="85504-687">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-687">Boolean</span></span>|<span data-ttu-id="85504-688">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="85504-688">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="85504-689">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="85504-689">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="85504-690">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-690">Boolean</span></span>|<span data-ttu-id="85504-691">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="85504-691">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="85504-692">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-692">internetSharingBlocked</span></span>|<span data-ttu-id="85504-693">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-693">Boolean</span></span>|<span data-ttu-id="85504-694">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="85504-694">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="85504-695">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="85504-695">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="85504-696">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-696">Boolean</span></span>|<span data-ttu-id="85504-697">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="85504-697">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="85504-698">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="85504-698">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="85504-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-699">Boolean</span></span>|<span data-ttu-id="85504-700">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="85504-700">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="85504-701">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="85504-701">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="85504-702">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-702">Boolean</span></span>|<span data-ttu-id="85504-703">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="85504-703">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="85504-704">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="85504-704">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="85504-705">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-705">Boolean</span></span>|<span data-ttu-id="85504-706">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="85504-706">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="85504-707">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="85504-707">settingsBlockChangeRegion</span></span>|<span data-ttu-id="85504-708">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-708">Boolean</span></span>|<span data-ttu-id="85504-709">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="85504-709">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="85504-710">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="85504-710">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="85504-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-711">Boolean</span></span>|<span data-ttu-id="85504-712">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="85504-712">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="85504-713">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="85504-713">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="85504-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-714">Boolean</span></span>|<span data-ttu-id="85504-715">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="85504-715">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="85504-716">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-716">locationServicesBlocked</span></span>|<span data-ttu-id="85504-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-717">Boolean</span></span>|<span data-ttu-id="85504-718">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="85504-718">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="85504-719">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-719">microsoftAccountBlocked</span></span>|<span data-ttu-id="85504-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-720">Boolean</span></span>|<span data-ttu-id="85504-721">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="85504-721">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="85504-722">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="85504-722">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="85504-723">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-723">Boolean</span></span>|<span data-ttu-id="85504-724">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="85504-724">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="85504-725">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-725">nfcBlocked</span></span>|<span data-ttu-id="85504-726">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-726">Boolean</span></span>|<span data-ttu-id="85504-727">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="85504-727">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="85504-728">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-728">resetProtectionModeBlocked</span></span>|<span data-ttu-id="85504-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-729">Boolean</span></span>|<span data-ttu-id="85504-730">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="85504-730">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="85504-731">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-731">screenCaptureBlocked</span></span>|<span data-ttu-id="85504-732">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-732">Boolean</span></span>|<span data-ttu-id="85504-733">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="85504-733">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="85504-734">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="85504-734">storageBlockRemovableStorage</span></span>|<span data-ttu-id="85504-735">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-735">Boolean</span></span>|<span data-ttu-id="85504-736">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="85504-736">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="85504-737">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="85504-737">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="85504-738">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-738">Boolean</span></span>|<span data-ttu-id="85504-739">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="85504-739">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="85504-740">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-740">usbBlocked</span></span>|<span data-ttu-id="85504-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-741">Boolean</span></span>|<span data-ttu-id="85504-742">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="85504-742">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="85504-743">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-743">voiceRecordingBlocked</span></span>|<span data-ttu-id="85504-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-744">Boolean</span></span>|<span data-ttu-id="85504-745">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="85504-745">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="85504-746">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="85504-746">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="85504-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-747">Boolean</span></span>|<span data-ttu-id="85504-748">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="85504-748">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="85504-749">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="85504-749">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="85504-750">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-750">wiFiBlocked</span></span>|<span data-ttu-id="85504-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-751">Boolean</span></span>|<span data-ttu-id="85504-752">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="85504-752">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="85504-753">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="85504-753">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="85504-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-754">Boolean</span></span>|<span data-ttu-id="85504-755">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="85504-755">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="85504-756">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="85504-756">wiFiScanInterval</span></span>|<span data-ttu-id="85504-757">Int32</span><span class="sxs-lookup"><span data-stu-id="85504-757">Int32</span></span>|<span data-ttu-id="85504-758">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="85504-758">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="85504-759">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="85504-759">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="85504-760">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="85504-760">Valid values 1 to 500</span></span>|
|<span data-ttu-id="85504-761">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="85504-761">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="85504-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-762">Boolean</span></span>|<span data-ttu-id="85504-763">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="85504-763">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="85504-764">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="85504-764">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="85504-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-765">Boolean</span></span>|<span data-ttu-id="85504-766">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="85504-766">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="85504-767">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="85504-767">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="85504-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-768">Boolean</span></span>|<span data-ttu-id="85504-769">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="85504-769">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="85504-770">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-770">windowsStoreBlocked</span></span>|<span data-ttu-id="85504-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-771">Boolean</span></span>|<span data-ttu-id="85504-772">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="85504-772">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="85504-773">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="85504-773">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="85504-774">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="85504-774">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="85504-775">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="85504-775">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="85504-776">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="85504-776">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="85504-777">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="85504-777">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="85504-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-778">Boolean</span></span>|<span data-ttu-id="85504-779">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="85504-779">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="85504-780">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="85504-780">developerUnlockSetting</span></span>|[<span data-ttu-id="85504-781">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="85504-781">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="85504-782">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="85504-782">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="85504-783">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="85504-783">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="85504-784">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="85504-784">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="85504-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-785">Boolean</span></span>|<span data-ttu-id="85504-786">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="85504-786">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="85504-787">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="85504-787">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="85504-788">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-788">Boolean</span></span>|<span data-ttu-id="85504-789">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="85504-789">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="85504-790">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="85504-790">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="85504-791">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-791">Boolean</span></span>|<span data-ttu-id="85504-792">指示是否启用“仅限私人应用商店”。</span><span class="sxs-lookup"><span data-stu-id="85504-792">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="85504-793">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="85504-793">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="85504-794">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-794">Boolean</span></span>|<span data-ttu-id="85504-795">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="85504-795">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="85504-796">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="85504-796">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="85504-797">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-797">Boolean</span></span>|<span data-ttu-id="85504-798">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="85504-798">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="85504-799">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="85504-799">gameDvrBlocked</span></span>|<span data-ttu-id="85504-800">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-800">Boolean</span></span>|<span data-ttu-id="85504-801">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="85504-801">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="85504-802">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="85504-802">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="85504-803">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-803">Boolean</span></span>|<span data-ttu-id="85504-804">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="85504-804">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="85504-805">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="85504-805">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="85504-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-806">Boolean</span></span>|<span data-ttu-id="85504-807">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="85504-807">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="85504-808">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="85504-808">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="85504-809">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-809">Boolean</span></span>|<span data-ttu-id="85504-810">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="85504-810">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="85504-811">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="85504-811">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="85504-812">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-812">Boolean</span></span>|<span data-ttu-id="85504-813">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="85504-813">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="85504-814">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="85504-814">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="85504-815">Boolean</span><span class="sxs-lookup"><span data-stu-id="85504-815">Boolean</span></span>|<span data-ttu-id="85504-816">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="85504-816">Whether the device is required to connect to the network.</span></span>|



## <a name="response"></a><span data-ttu-id="85504-817">响应</span><span class="sxs-lookup"><span data-stu-id="85504-817">Response</span></span>
<span data-ttu-id="85504-818">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85504-818">If successful, this method returns a `201 Created` response code and a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85504-819">示例</span><span class="sxs-lookup"><span data-stu-id="85504-819">Example</span></span>

### <a name="request"></a><span data-ttu-id="85504-820">请求</span><span class="sxs-lookup"><span data-stu-id="85504-820">Request</span></span>
<span data-ttu-id="85504-821">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85504-821">Here is an example of the request.</span></span>
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
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
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

### <a name="response"></a><span data-ttu-id="85504-822">响应</span><span class="sxs-lookup"><span data-stu-id="85504-822">Response</span></span>
<span data-ttu-id="85504-p158">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85504-p158">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
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



