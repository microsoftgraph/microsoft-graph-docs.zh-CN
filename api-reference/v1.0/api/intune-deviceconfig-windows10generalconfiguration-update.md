---
title: 更新 windows10GeneralConfiguration
description: 更新 windows10GeneralConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c664f6cf2c206b5c1b40ec209f05919884b87b78
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514019"
---
# <a name="update-windows10generalconfiguration"></a><span data-ttu-id="2c3b9-103">更新 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c3b9-103">Update windows10GeneralConfiguration</span></span>

<span data-ttu-id="2c3b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c3b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c3b9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c3b9-106">更新 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-106">Update the properties of a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c3b9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c3b9-107">Prerequisites</span></span>
<span data-ttu-id="2c3b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c3b9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c3b9-110">Permission type</span></span>|<span data-ttu-id="2c3b9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2c3b9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c3b9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c3b9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c3b9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c3b9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c3b9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c3b9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c3b9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-115">Not supported.</span></span>|
|<span data-ttu-id="2c3b9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c3b9-116">Application</span></span>|<span data-ttu-id="2c3b9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c3b9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c3b9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2c3b9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c3b9-119">Request headers</span></span>
|<span data-ttu-id="2c3b9-120">标头</span><span class="sxs-lookup"><span data-stu-id="2c3b9-120">Header</span></span>|<span data-ttu-id="2c3b9-121">值</span><span class="sxs-lookup"><span data-stu-id="2c3b9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c3b9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c3b9-122">Authorization</span></span>|<span data-ttu-id="2c3b9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c3b9-124">接受</span><span class="sxs-lookup"><span data-stu-id="2c3b9-124">Accept</span></span>|<span data-ttu-id="2c3b9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c3b9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c3b9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c3b9-126">Request body</span></span>
<span data-ttu-id="2c3b9-127">在请求正文中，提供 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-127">In the request body, supply a JSON representation for the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

<span data-ttu-id="2c3b9-128">下表显示了创建 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-128">The following table shows the properties that are required when you create the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>

|<span data-ttu-id="2c3b9-129">属性</span><span class="sxs-lookup"><span data-stu-id="2c3b9-129">Property</span></span>|<span data-ttu-id="2c3b9-130">类型</span><span class="sxs-lookup"><span data-stu-id="2c3b9-130">Type</span></span>|<span data-ttu-id="2c3b9-131">说明</span><span class="sxs-lookup"><span data-stu-id="2c3b9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c3b9-132">id</span><span class="sxs-lookup"><span data-stu-id="2c3b9-132">id</span></span>|<span data-ttu-id="2c3b9-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2c3b9-133">String</span></span>|<span data-ttu-id="2c3b9-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-134">Key of the entity.</span></span> <span data-ttu-id="2c3b9-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c3b9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c3b9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c3b9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2c3b9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c3b9-137">DateTimeOffset</span></span>|<span data-ttu-id="2c3b9-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2c3b9-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c3b9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c3b9-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c3b9-140">createdDateTime</span></span>|<span data-ttu-id="2c3b9-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c3b9-141">DateTimeOffset</span></span>|<span data-ttu-id="2c3b9-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-142">DateTime the object was created.</span></span> <span data-ttu-id="2c3b9-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c3b9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c3b9-144">说明</span><span class="sxs-lookup"><span data-stu-id="2c3b9-144">description</span></span>|<span data-ttu-id="2c3b9-145">String</span><span class="sxs-lookup"><span data-stu-id="2c3b9-145">String</span></span>|<span data-ttu-id="2c3b9-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2c3b9-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c3b9-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c3b9-148">displayName</span><span class="sxs-lookup"><span data-stu-id="2c3b9-148">displayName</span></span>|<span data-ttu-id="2c3b9-149">字符串</span><span class="sxs-lookup"><span data-stu-id="2c3b9-149">String</span></span>|<span data-ttu-id="2c3b9-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2c3b9-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c3b9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c3b9-152">version</span><span class="sxs-lookup"><span data-stu-id="2c3b9-152">version</span></span>|<span data-ttu-id="2c3b9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-153">Int32</span></span>|<span data-ttu-id="2c3b9-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-154">Version of the device configuration.</span></span> <span data-ttu-id="2c3b9-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c3b9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c3b9-156">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="2c3b9-156">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="2c3b9-157">字符串</span><span class="sxs-lookup"><span data-stu-id="2c3b9-157">String</span></span>|<span data-ttu-id="2c3b9-158">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-158">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="2c3b9-159">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="2c3b9-159">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="2c3b9-160">字符串</span><span class="sxs-lookup"><span data-stu-id="2c3b9-160">String</span></span>|<span data-ttu-id="2c3b9-161">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-161">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="2c3b9-162">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="2c3b9-162">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="2c3b9-163">字符串</span><span class="sxs-lookup"><span data-stu-id="2c3b9-163">String</span></span>|<span data-ttu-id="2c3b9-164">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-164">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="2c3b9-165">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2c3b9-165">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="2c3b9-166">字符串</span><span class="sxs-lookup"><span data-stu-id="2c3b9-166">String</span></span>|<span data-ttu-id="2c3b9-167">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-167">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="2c3b9-168">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="2c3b9-168">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="2c3b9-169">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-169">Int32</span></span>|<span data-ttu-id="2c3b9-170">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-170">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="2c3b9-171">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-171">This is a mobile only setting.</span></span> <span data-ttu-id="2c3b9-172">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="2c3b9-172">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="2c3b9-173">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2c3b9-173">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="2c3b9-174">字符串</span><span class="sxs-lookup"><span data-stu-id="2c3b9-174">String</span></span>|<span data-ttu-id="2c3b9-175">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-175">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="2c3b9-176">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="2c3b9-176">searchBlockDiacritics</span></span>|<span data-ttu-id="2c3b9-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-177">Boolean</span></span>|<span data-ttu-id="2c3b9-178">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-178">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="2c3b9-179">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="2c3b9-179">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="2c3b9-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-180">Boolean</span></span>|<span data-ttu-id="2c3b9-181">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-181">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="2c3b9-182">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="2c3b9-182">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="2c3b9-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-183">Boolean</span></span>|<span data-ttu-id="2c3b9-184">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-184">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="2c3b9-185">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="2c3b9-185">searchEnableRemoteQueries</span></span>|<span data-ttu-id="2c3b9-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-186">Boolean</span></span>|<span data-ttu-id="2c3b9-187">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-187">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="2c3b9-188">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="2c3b9-188">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="2c3b9-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-189">Boolean</span></span>|<span data-ttu-id="2c3b9-190">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-190">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="2c3b9-191">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="2c3b9-191">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="2c3b9-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-192">Boolean</span></span>|<span data-ttu-id="2c3b9-193">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-193">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="2c3b9-194">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="2c3b9-194">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="2c3b9-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-195">Boolean</span></span>|<span data-ttu-id="2c3b9-196">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-196">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="2c3b9-197">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="2c3b9-197">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="2c3b9-198">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="2c3b9-198">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="2c3b9-199">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-199">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="2c3b9-200">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-200">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="2c3b9-201">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="2c3b9-201">oneDriveDisableFileSync</span></span>|<span data-ttu-id="2c3b9-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-202">Boolean</span></span>|<span data-ttu-id="2c3b9-203">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-203">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="2c3b9-204">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="2c3b9-204">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="2c3b9-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-205">Boolean</span></span>|<span data-ttu-id="2c3b9-206">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-206">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="2c3b9-207">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="2c3b9-207">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="2c3b9-208">字符串</span><span class="sxs-lookup"><span data-stu-id="2c3b9-208">String</span></span>|<span data-ttu-id="2c3b9-209">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-209">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="2c3b9-210">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="2c3b9-210">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="2c3b9-211">String</span><span class="sxs-lookup"><span data-stu-id="2c3b9-211">String</span></span>|<span data-ttu-id="2c3b9-212">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-212">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="2c3b9-213">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="2c3b9-213">bluetoothAllowedServices</span></span>|<span data-ttu-id="2c3b9-214">String 集合</span><span class="sxs-lookup"><span data-stu-id="2c3b9-214">String collection</span></span>|<span data-ttu-id="2c3b9-215">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-215">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="2c3b9-216">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="2c3b9-216">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="2c3b9-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-217">Boolean</span></span>|<span data-ttu-id="2c3b9-218">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-218">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="2c3b9-219">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="2c3b9-219">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="2c3b9-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-220">Boolean</span></span>|<span data-ttu-id="2c3b9-221">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-221">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="2c3b9-222">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="2c3b9-222">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="2c3b9-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-223">Boolean</span></span>|<span data-ttu-id="2c3b9-224">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-224">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="2c3b9-225">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="2c3b9-225">edgeBlockAutofill</span></span>|<span data-ttu-id="2c3b9-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-226">Boolean</span></span>|<span data-ttu-id="2c3b9-227">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-227">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="2c3b9-228">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-228">edgeBlocked</span></span>|<span data-ttu-id="2c3b9-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-229">Boolean</span></span>|<span data-ttu-id="2c3b9-230">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-230">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="2c3b9-231">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="2c3b9-231">edgeCookiePolicy</span></span>|[<span data-ttu-id="2c3b9-232">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="2c3b9-232">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="2c3b9-233">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-233">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="2c3b9-234">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-234">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="2c3b9-235">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="2c3b9-235">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="2c3b9-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-236">Boolean</span></span>|<span data-ttu-id="2c3b9-237">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-237">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="2c3b9-238">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="2c3b9-238">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="2c3b9-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-239">Boolean</span></span>|<span data-ttu-id="2c3b9-240">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-240">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="2c3b9-241">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="2c3b9-241">edgeBlockExtensions</span></span>|<span data-ttu-id="2c3b9-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-242">Boolean</span></span>|<span data-ttu-id="2c3b9-243">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-243">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="2c3b9-244">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="2c3b9-244">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="2c3b9-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-245">Boolean</span></span>|<span data-ttu-id="2c3b9-246">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-246">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="2c3b9-247">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="2c3b9-247">edgeBlockJavaScript</span></span>|<span data-ttu-id="2c3b9-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-248">Boolean</span></span>|<span data-ttu-id="2c3b9-249">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-249">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="2c3b9-250">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="2c3b9-250">edgeBlockPasswordManager</span></span>|<span data-ttu-id="2c3b9-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-251">Boolean</span></span>|<span data-ttu-id="2c3b9-252">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-252">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="2c3b9-253">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="2c3b9-253">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="2c3b9-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-254">Boolean</span></span>|<span data-ttu-id="2c3b9-255">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-255">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="2c3b9-256">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-256">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="2c3b9-257">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="2c3b9-257">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="2c3b9-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-258">Boolean</span></span>|<span data-ttu-id="2c3b9-259">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-259">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="2c3b9-260">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-260">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="2c3b9-261">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="2c3b9-261">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="2c3b9-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-262">Boolean</span></span>|<span data-ttu-id="2c3b9-263">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-263">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="2c3b9-264">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="2c3b9-264">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="2c3b9-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-265">Boolean</span></span>|<span data-ttu-id="2c3b9-266">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-266">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="2c3b9-267">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-267">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="2c3b9-268">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-268">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="2c3b9-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-269">Boolean</span></span>|<span data-ttu-id="2c3b9-270">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-270">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="2c3b9-271">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-271">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="2c3b9-272">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="2c3b9-272">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="2c3b9-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-273">Boolean</span></span>|<span data-ttu-id="2c3b9-274">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-274">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="2c3b9-275">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="2c3b9-275">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="2c3b9-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-276">Boolean</span></span>|<span data-ttu-id="2c3b9-277">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-277">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="2c3b9-278">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-278">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="2c3b9-279">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="2c3b9-279">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="2c3b9-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-280">Boolean</span></span>|<span data-ttu-id="2c3b9-281">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-281">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="2c3b9-282">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="2c3b9-282">cellularBlockVpn</span></span>|<span data-ttu-id="2c3b9-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-283">Boolean</span></span>|<span data-ttu-id="2c3b9-284">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-284">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="2c3b9-285">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="2c3b9-285">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="2c3b9-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-286">Boolean</span></span>|<span data-ttu-id="2c3b9-287">通过手机网络漫游时是否阻止用户使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-287">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="2c3b9-288">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="2c3b9-288">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="2c3b9-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-289">Boolean</span></span>|<span data-ttu-id="2c3b9-290">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-290">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="2c3b9-291">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="2c3b9-291">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="2c3b9-292">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-292">Int32</span></span>|<span data-ttu-id="2c3b9-293">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-293">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="2c3b9-294">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="2c3b9-294">Valid values 0 to 90</span></span>|
|<span data-ttu-id="2c3b9-295">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="2c3b9-295">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="2c3b9-296">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="2c3b9-296">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="2c3b9-297">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-297">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="2c3b9-298">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="2c3b9-298">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="2c3b9-299">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="2c3b9-299">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="2c3b9-300">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-300">Defender day of the week for the system scan.</span></span> <span data-ttu-id="2c3b9-301">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-301">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="2c3b9-302">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="2c3b9-302">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="2c3b9-303">String collection</span><span class="sxs-lookup"><span data-stu-id="2c3b9-303">String collection</span></span>|<span data-ttu-id="2c3b9-304">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-304">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="2c3b9-305">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="2c3b9-305">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="2c3b9-306">String collection</span><span class="sxs-lookup"><span data-stu-id="2c3b9-306">String collection</span></span>|<span data-ttu-id="2c3b9-307">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-307">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="2c3b9-308">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="2c3b9-308">defenderScanMaxCpu</span></span>|<span data-ttu-id="2c3b9-309">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-309">Int32</span></span>|<span data-ttu-id="2c3b9-310">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-310">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="2c3b9-311">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="2c3b9-311">Valid values 0 to 100</span></span>|
|<span data-ttu-id="2c3b9-312">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="2c3b9-312">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="2c3b9-313">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="2c3b9-313">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="2c3b9-314">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-314">Value for monitoring file activity.</span></span> <span data-ttu-id="2c3b9-315">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-315">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="2c3b9-316">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="2c3b9-316">defenderProcessesToExclude</span></span>|<span data-ttu-id="2c3b9-317">String 集合</span><span class="sxs-lookup"><span data-stu-id="2c3b9-317">String collection</span></span>|<span data-ttu-id="2c3b9-318">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-318">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="2c3b9-319">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="2c3b9-319">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="2c3b9-320">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="2c3b9-320">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="2c3b9-321">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-321">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="2c3b9-322">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-322">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="2c3b9-323">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="2c3b9-323">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="2c3b9-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-324">Boolean</span></span>|<span data-ttu-id="2c3b9-325">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-325">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="2c3b9-326">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="2c3b9-326">defenderRequireCloudProtection</span></span>|<span data-ttu-id="2c3b9-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-327">Boolean</span></span>|<span data-ttu-id="2c3b9-328">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-328">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="2c3b9-329">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="2c3b9-329">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="2c3b9-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-330">Boolean</span></span>|<span data-ttu-id="2c3b9-331">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-331">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="2c3b9-332">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="2c3b9-332">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="2c3b9-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-333">Boolean</span></span>|<span data-ttu-id="2c3b9-334">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-334">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="2c3b9-335">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="2c3b9-335">defenderScanArchiveFiles</span></span>|<span data-ttu-id="2c3b9-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-336">Boolean</span></span>|<span data-ttu-id="2c3b9-337">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-337">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="2c3b9-338">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="2c3b9-338">defenderScanDownloads</span></span>|<span data-ttu-id="2c3b9-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-339">Boolean</span></span>|<span data-ttu-id="2c3b9-340">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-340">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="2c3b9-341">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="2c3b9-341">defenderScanNetworkFiles</span></span>|<span data-ttu-id="2c3b9-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-342">Boolean</span></span>|<span data-ttu-id="2c3b9-343">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-343">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="2c3b9-344">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="2c3b9-344">defenderScanIncomingMail</span></span>|<span data-ttu-id="2c3b9-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-345">Boolean</span></span>|<span data-ttu-id="2c3b9-346">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-346">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="2c3b9-347">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="2c3b9-347">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="2c3b9-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-348">Boolean</span></span>|<span data-ttu-id="2c3b9-349">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-349">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="2c3b9-350">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="2c3b9-350">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="2c3b9-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-351">Boolean</span></span>|<span data-ttu-id="2c3b9-352">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-352">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="2c3b9-353">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="2c3b9-353">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="2c3b9-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-354">Boolean</span></span>|<span data-ttu-id="2c3b9-355">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-355">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="2c3b9-356">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="2c3b9-356">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="2c3b9-357">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-357">Int32</span></span>|<span data-ttu-id="2c3b9-358">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-358">The signature update interval in hours.</span></span> <span data-ttu-id="2c3b9-359">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-359">Specify 0 not to check.</span></span> <span data-ttu-id="2c3b9-360">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="2c3b9-360">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2c3b9-361">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="2c3b9-361">defenderScanType</span></span>|[<span data-ttu-id="2c3b9-362">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="2c3b9-362">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="2c3b9-363">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-363">The defender system scan type.</span></span> <span data-ttu-id="2c3b9-364">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-364">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="2c3b9-365">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="2c3b9-365">defenderScheduledScanTime</span></span>|<span data-ttu-id="2c3b9-366">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2c3b9-366">TimeOfDay</span></span>|<span data-ttu-id="2c3b9-367">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-367">The defender time for the system scan.</span></span>|
|<span data-ttu-id="2c3b9-368">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="2c3b9-368">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="2c3b9-369">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2c3b9-369">TimeOfDay</span></span>|<span data-ttu-id="2c3b9-370">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-370">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="2c3b9-371">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="2c3b9-371">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="2c3b9-372">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="2c3b9-372">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="2c3b9-373">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-373">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="2c3b9-374">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-374">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="2c3b9-375">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c3b9-375">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="2c3b9-376">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-376">Boolean</span></span>|<span data-ttu-id="2c3b9-377">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-377">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="2c3b9-378">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-378">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="2c3b9-379">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="2c3b9-379">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="2c3b9-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-380">Boolean</span></span>|<span data-ttu-id="2c3b9-381">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-381">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="2c3b9-382">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="2c3b9-382">lockScreenBlockCortana</span></span>|<span data-ttu-id="2c3b9-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-383">Boolean</span></span>|<span data-ttu-id="2c3b9-384">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-384">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="2c3b9-385">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="2c3b9-385">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="2c3b9-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-386">Boolean</span></span>|<span data-ttu-id="2c3b9-387">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-387">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="2c3b9-388">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="2c3b9-388">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="2c3b9-389">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-389">Int32</span></span>|<span data-ttu-id="2c3b9-390">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-390">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="2c3b9-391">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-391">Supported values are 11-1800.</span></span> <span data-ttu-id="2c3b9-392">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="2c3b9-392">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="2c3b9-393">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2c3b9-393">passwordBlockSimple</span></span>|<span data-ttu-id="2c3b9-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-394">Boolean</span></span>|<span data-ttu-id="2c3b9-395">指定是否允许使用 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-395">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="2c3b9-396">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-396">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="2c3b9-397">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2c3b9-397">passwordExpirationDays</span></span>|<span data-ttu-id="2c3b9-398">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-398">Int32</span></span>|<span data-ttu-id="2c3b9-399">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-399">The password expiration in days.</span></span> <span data-ttu-id="2c3b9-400">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="2c3b9-400">Valid values 0 to 730</span></span>|
|<span data-ttu-id="2c3b9-401">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2c3b9-401">passwordMinimumLength</span></span>|<span data-ttu-id="2c3b9-402">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-402">Int32</span></span>|<span data-ttu-id="2c3b9-403">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-403">The minimum password length.</span></span> <span data-ttu-id="2c3b9-404">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="2c3b9-404">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2c3b9-405">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2c3b9-405">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2c3b9-406">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-406">Int32</span></span>|<span data-ttu-id="2c3b9-407">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-407">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2c3b9-408">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2c3b9-408">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2c3b9-409">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-409">Int32</span></span>|<span data-ttu-id="2c3b9-410">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-410">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2c3b9-411">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2c3b9-411">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2c3b9-412">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-412">Int32</span></span>|<span data-ttu-id="2c3b9-413">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-413">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="2c3b9-414">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="2c3b9-414">Valid values 0 to 50</span></span>|
|<span data-ttu-id="2c3b9-415">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2c3b9-415">passwordRequired</span></span>|<span data-ttu-id="2c3b9-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-416">Boolean</span></span>|<span data-ttu-id="2c3b9-417">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-417">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="2c3b9-418">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="2c3b9-418">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="2c3b9-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-419">Boolean</span></span>|<span data-ttu-id="2c3b9-420">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-420">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="2c3b9-421">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2c3b9-421">passwordRequiredType</span></span>|[<span data-ttu-id="2c3b9-422">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2c3b9-422">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2c3b9-423">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-423">The required password type.</span></span> <span data-ttu-id="2c3b9-424">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-424">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2c3b9-425">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2c3b9-425">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2c3b9-426">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-426">Int32</span></span>|<span data-ttu-id="2c3b9-427">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-427">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="2c3b9-428">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="2c3b9-428">Valid values 0 to 999</span></span>|
|<span data-ttu-id="2c3b9-429">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="2c3b9-429">privacyAdvertisingId</span></span>|[<span data-ttu-id="2c3b9-430">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-430">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="2c3b9-431">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-431">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="2c3b9-432">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-432">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="2c3b9-433">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-433">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="2c3b9-434">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="2c3b9-434">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="2c3b9-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-435">Boolean</span></span>|<span data-ttu-id="2c3b9-436">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-436">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="2c3b9-437">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="2c3b9-437">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="2c3b9-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-438">Boolean</span></span>|<span data-ttu-id="2c3b9-439">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-439">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="2c3b9-440">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="2c3b9-440">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="2c3b9-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-441">Boolean</span></span>|<span data-ttu-id="2c3b9-442">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-442">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="2c3b9-443">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="2c3b9-443">startMenuAppListVisibility</span></span>|[<span data-ttu-id="2c3b9-444">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="2c3b9-444">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="2c3b9-445">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-445">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="2c3b9-446">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-446">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="2c3b9-447">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="2c3b9-447">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="2c3b9-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-448">Boolean</span></span>|<span data-ttu-id="2c3b9-449">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-449">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="2c3b9-450">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="2c3b9-450">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="2c3b9-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-451">Boolean</span></span>|<span data-ttu-id="2c3b9-452">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-452">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="2c3b9-453">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="2c3b9-453">startMenuHideHibernate</span></span>|<span data-ttu-id="2c3b9-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-454">Boolean</span></span>|<span data-ttu-id="2c3b9-455">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-455">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="2c3b9-456">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="2c3b9-456">startMenuHideLock</span></span>|<span data-ttu-id="2c3b9-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-457">Boolean</span></span>|<span data-ttu-id="2c3b9-458">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-458">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="2c3b9-459">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="2c3b9-459">startMenuHidePowerButton</span></span>|<span data-ttu-id="2c3b9-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-460">Boolean</span></span>|<span data-ttu-id="2c3b9-461">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-461">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="2c3b9-462">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="2c3b9-462">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="2c3b9-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-463">Boolean</span></span>|<span data-ttu-id="2c3b9-464">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-464">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="2c3b9-465">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="2c3b9-465">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="2c3b9-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-466">Boolean</span></span>|<span data-ttu-id="2c3b9-467">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-467">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="2c3b9-468">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="2c3b9-468">startMenuHideRestartOptions</span></span>|<span data-ttu-id="2c3b9-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-469">Boolean</span></span>|<span data-ttu-id="2c3b9-470">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-470">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="2c3b9-471">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="2c3b9-471">startMenuHideShutDown</span></span>|<span data-ttu-id="2c3b9-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-472">Boolean</span></span>|<span data-ttu-id="2c3b9-473">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-473">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="2c3b9-474">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="2c3b9-474">startMenuHideSignOut</span></span>|<span data-ttu-id="2c3b9-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-475">Boolean</span></span>|<span data-ttu-id="2c3b9-476">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-476">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="2c3b9-477">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="2c3b9-477">startMenuHideSleep</span></span>|<span data-ttu-id="2c3b9-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-478">Boolean</span></span>|<span data-ttu-id="2c3b9-479">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-479">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="2c3b9-480">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="2c3b9-480">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="2c3b9-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-481">Boolean</span></span>|<span data-ttu-id="2c3b9-482">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-482">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="2c3b9-483">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="2c3b9-483">startMenuHideUserTile</span></span>|<span data-ttu-id="2c3b9-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-484">Boolean</span></span>|<span data-ttu-id="2c3b9-485">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-485">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="2c3b9-486">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="2c3b9-486">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="2c3b9-487">Binary</span><span class="sxs-lookup"><span data-stu-id="2c3b9-487">Binary</span></span>|<span data-ttu-id="2c3b9-488">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-488">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="2c3b9-489">“开始”菜单布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-489">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="2c3b9-490">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-490">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="2c3b9-491">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-491">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="2c3b9-492">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-492">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="2c3b9-493">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="2c3b9-493">startMenuLayoutXml</span></span>|<span data-ttu-id="2c3b9-494">Binary</span><span class="sxs-lookup"><span data-stu-id="2c3b9-494">Binary</span></span>|<span data-ttu-id="2c3b9-495">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-495">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="2c3b9-496">通过基于布局修改架构指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-496">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="2c3b9-497">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-497">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="2c3b9-498">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="2c3b9-498">startMenuMode</span></span>|[<span data-ttu-id="2c3b9-499">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="2c3b9-499">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="2c3b9-500">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-500">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="2c3b9-501">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-501">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="2c3b9-502">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="2c3b9-502">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="2c3b9-503">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-503">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="2c3b9-504">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-504">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="2c3b9-505">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-505">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="2c3b9-506">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="2c3b9-506">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="2c3b9-507">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-507">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="2c3b9-508">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-508">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="2c3b9-509">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-509">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="2c3b9-510">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="2c3b9-510">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="2c3b9-511">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-511">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="2c3b9-512">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-512">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="2c3b9-513">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-513">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="2c3b9-514">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="2c3b9-514">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="2c3b9-515">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-515">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="2c3b9-516">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-516">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="2c3b9-517">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-517">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="2c3b9-518">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="2c3b9-518">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="2c3b9-519">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-519">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="2c3b9-520">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-520">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="2c3b9-521">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-521">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="2c3b9-522">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="2c3b9-522">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="2c3b9-523">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-523">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="2c3b9-524">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-524">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="2c3b9-525">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-525">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="2c3b9-526">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="2c3b9-526">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="2c3b9-527">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-527">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="2c3b9-528">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-528">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="2c3b9-529">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-529">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="2c3b9-530">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="2c3b9-530">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="2c3b9-531">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-531">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="2c3b9-532">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-532">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="2c3b9-533">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-533">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="2c3b9-534">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="2c3b9-534">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="2c3b9-535">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-535">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="2c3b9-536">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-536">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="2c3b9-537">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-537">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="2c3b9-538">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="2c3b9-538">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="2c3b9-539">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-539">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="2c3b9-540">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-540">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="2c3b9-541">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-541">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="2c3b9-542">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="2c3b9-542">settingsBlockSettingsApp</span></span>|<span data-ttu-id="2c3b9-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-543">Boolean</span></span>|<span data-ttu-id="2c3b9-544">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-544">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="2c3b9-545">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-545">settingsBlockSystemPage</span></span>|<span data-ttu-id="2c3b9-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-546">Boolean</span></span>|<span data-ttu-id="2c3b9-547">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-547">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="2c3b9-548">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-548">settingsBlockDevicesPage</span></span>|<span data-ttu-id="2c3b9-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-549">Boolean</span></span>|<span data-ttu-id="2c3b9-550">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-550">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="2c3b9-551">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-551">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="2c3b9-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-552">Boolean</span></span>|<span data-ttu-id="2c3b9-553">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-553">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="2c3b9-554">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-554">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="2c3b9-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-555">Boolean</span></span>|<span data-ttu-id="2c3b9-556">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-556">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="2c3b9-557">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-557">settingsBlockAccountsPage</span></span>|<span data-ttu-id="2c3b9-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-558">Boolean</span></span>|<span data-ttu-id="2c3b9-559">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-559">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="2c3b9-560">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-560">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="2c3b9-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-561">Boolean</span></span>|<span data-ttu-id="2c3b9-562">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-562">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="2c3b9-563">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-563">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="2c3b9-564">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-564">Boolean</span></span>|<span data-ttu-id="2c3b9-565">指示是否阻止在“设置”应用中访问“轻松使用”。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-565">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="2c3b9-566">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-566">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="2c3b9-567">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-567">Boolean</span></span>|<span data-ttu-id="2c3b9-568">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-568">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="2c3b9-569">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-569">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="2c3b9-570">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-570">Boolean</span></span>|<span data-ttu-id="2c3b9-571">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-571">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="2c3b9-572">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-572">settingsBlockAppsPage</span></span>|<span data-ttu-id="2c3b9-573">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-573">Boolean</span></span>|<span data-ttu-id="2c3b9-574">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-574">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="2c3b9-575">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-575">settingsBlockGamingPage</span></span>|<span data-ttu-id="2c3b9-576">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-576">Boolean</span></span>|<span data-ttu-id="2c3b9-577">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-577">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="2c3b9-578">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="2c3b9-578">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="2c3b9-579">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-579">Boolean</span></span>|<span data-ttu-id="2c3b9-580">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-580">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="2c3b9-581">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-581">windowsSpotlightBlocked</span></span>|<span data-ttu-id="2c3b9-582">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-582">Boolean</span></span>|<span data-ttu-id="2c3b9-583">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="2c3b9-583">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="2c3b9-584">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="2c3b9-584">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="2c3b9-585">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-585">Boolean</span></span>|<span data-ttu-id="2c3b9-586">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="2c3b9-586">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="2c3b9-587">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="2c3b9-587">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="2c3b9-588">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-588">Boolean</span></span>|<span data-ttu-id="2c3b9-589">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-589">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="2c3b9-590">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="2c3b9-590">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="2c3b9-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-591">Boolean</span></span>|<span data-ttu-id="2c3b9-592">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="2c3b9-592">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="2c3b9-593">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="2c3b9-593">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="2c3b9-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-594">Boolean</span></span>|<span data-ttu-id="2c3b9-595">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="2c3b9-595">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="2c3b9-596">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="2c3b9-596">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="2c3b9-597">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-597">Boolean</span></span>|<span data-ttu-id="2c3b9-598">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-598">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="2c3b9-599">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="2c3b9-599">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="2c3b9-600">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="2c3b9-600">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="2c3b9-601">指定聚光灯的类型。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-601">Specifies the type of Spotlight.</span></span> <span data-ttu-id="2c3b9-602">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-602">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="2c3b9-603">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="2c3b9-603">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="2c3b9-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-604">Boolean</span></span>|<span data-ttu-id="2c3b9-605">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-605">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="2c3b9-606">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-606">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="2c3b9-607">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="2c3b9-607">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="2c3b9-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-608">Boolean</span></span>|<span data-ttu-id="2c3b9-609">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-609">Disable automatic detection of settings.</span></span> <span data-ttu-id="2c3b9-610">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-610">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="2c3b9-611">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="2c3b9-611">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="2c3b9-612">String</span><span class="sxs-lookup"><span data-stu-id="2c3b9-612">String</span></span>|<span data-ttu-id="2c3b9-613">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-613">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="2c3b9-614">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="2c3b9-614">networkProxyServer</span></span>|[<span data-ttu-id="2c3b9-615">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="2c3b9-615">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="2c3b9-616">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-616">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="2c3b9-617">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="2c3b9-617">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="2c3b9-618">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-618">Boolean</span></span>|<span data-ttu-id="2c3b9-619">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-619">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="2c3b9-620">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-620">antiTheftModeBlocked</span></span>|<span data-ttu-id="2c3b9-621">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-621">Boolean</span></span>|<span data-ttu-id="2c3b9-622">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-622">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="2c3b9-623">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-623">bluetoothBlocked</span></span>|<span data-ttu-id="2c3b9-624">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-624">Boolean</span></span>|<span data-ttu-id="2c3b9-625">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-625">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="2c3b9-626">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-626">cameraBlocked</span></span>|<span data-ttu-id="2c3b9-627">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-627">Boolean</span></span>|<span data-ttu-id="2c3b9-628">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-628">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="2c3b9-629">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-629">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="2c3b9-630">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-630">Boolean</span></span>|<span data-ttu-id="2c3b9-631">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-631">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="2c3b9-632">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="2c3b9-632">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="2c3b9-633">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-633">Boolean</span></span>|<span data-ttu-id="2c3b9-634">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-634">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="2c3b9-635">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-635">copyPasteBlocked</span></span>|<span data-ttu-id="2c3b9-636">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-636">Boolean</span></span>|<span data-ttu-id="2c3b9-637">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-637">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="2c3b9-638">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-638">cortanaBlocked</span></span>|<span data-ttu-id="2c3b9-639">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-639">Boolean</span></span>|<span data-ttu-id="2c3b9-640">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-640">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="2c3b9-641">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="2c3b9-641">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="2c3b9-642">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-642">Boolean</span></span>|<span data-ttu-id="2c3b9-643">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-643">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="2c3b9-644">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="2c3b9-644">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="2c3b9-645">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-645">Boolean</span></span>|<span data-ttu-id="2c3b9-646">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-646">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="2c3b9-647">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="2c3b9-647">safeSearchFilter</span></span>|[<span data-ttu-id="2c3b9-648">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="2c3b9-648">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="2c3b9-649">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-649">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="2c3b9-650">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-650">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="2c3b9-651">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="2c3b9-651">edgeBlockPopups</span></span>|<span data-ttu-id="2c3b9-652">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-652">Boolean</span></span>|<span data-ttu-id="2c3b9-653">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-653">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="2c3b9-654">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="2c3b9-654">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="2c3b9-655">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-655">Boolean</span></span>|<span data-ttu-id="2c3b9-656">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-656">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="2c3b9-657">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="2c3b9-657">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="2c3b9-658">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-658">Boolean</span></span>|<span data-ttu-id="2c3b9-659">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-659">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="2c3b9-660">注意：此属性的名称是误导性的;属性已过时，请改用 EdgeSendIntranetTrafficToInternetExplorer。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-660">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="2c3b9-661">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="2c3b9-661">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="2c3b9-662">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-662">Boolean</span></span>|<span data-ttu-id="2c3b9-663">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-663">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="2c3b9-664">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="2c3b9-664">edgeRequireSmartScreen</span></span>|<span data-ttu-id="2c3b9-665">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-665">Boolean</span></span>|<span data-ttu-id="2c3b9-666">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-666">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="2c3b9-667">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="2c3b9-667">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="2c3b9-668">字符串</span><span class="sxs-lookup"><span data-stu-id="2c3b9-668">String</span></span>|<span data-ttu-id="2c3b9-669">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-669">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="2c3b9-670">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-670">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="2c3b9-671">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="2c3b9-671">edgeFirstRunUrl</span></span>|<span data-ttu-id="2c3b9-672">String</span><span class="sxs-lookup"><span data-stu-id="2c3b9-672">String</span></span>|<span data-ttu-id="2c3b9-673">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-673">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="2c3b9-674">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="2c3b9-674">edgeSearchEngine</span></span>|[<span data-ttu-id="2c3b9-675">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="2c3b9-675">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="2c3b9-676">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-676">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="2c3b9-677">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-677">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="2c3b9-678">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="2c3b9-678">edgeHomepageUrls</span></span>|<span data-ttu-id="2c3b9-679">String 集合</span><span class="sxs-lookup"><span data-stu-id="2c3b9-679">String collection</span></span>|<span data-ttu-id="2c3b9-680">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-680">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="2c3b9-681">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="2c3b9-681">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="2c3b9-682">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-682">Boolean</span></span>|<span data-ttu-id="2c3b9-683">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-683">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="2c3b9-684">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="2c3b9-684">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="2c3b9-685">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-685">Boolean</span></span>|<span data-ttu-id="2c3b9-686">指示用户是否可以替代有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-686">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="2c3b9-687">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="2c3b9-687">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="2c3b9-688">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-688">Boolean</span></span>|<span data-ttu-id="2c3b9-689">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="2c3b9-689">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="2c3b9-690">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="2c3b9-690">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="2c3b9-691">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-691">Boolean</span></span>|<span data-ttu-id="2c3b9-692">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="2c3b9-692">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="2c3b9-693">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-693">internetSharingBlocked</span></span>|<span data-ttu-id="2c3b9-694">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-694">Boolean</span></span>|<span data-ttu-id="2c3b9-695">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-695">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="2c3b9-696">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-696">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="2c3b9-697">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-697">Boolean</span></span>|<span data-ttu-id="2c3b9-698">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-698">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="2c3b9-699">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-699">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="2c3b9-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-700">Boolean</span></span>|<span data-ttu-id="2c3b9-701">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-701">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="2c3b9-702">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="2c3b9-702">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="2c3b9-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-703">Boolean</span></span>|<span data-ttu-id="2c3b9-704">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-704">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="2c3b9-705">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="2c3b9-705">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="2c3b9-706">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-706">Boolean</span></span>|<span data-ttu-id="2c3b9-707">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-707">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="2c3b9-708">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="2c3b9-708">settingsBlockChangeRegion</span></span>|<span data-ttu-id="2c3b9-709">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-709">Boolean</span></span>|<span data-ttu-id="2c3b9-710">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-710">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="2c3b9-711">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-711">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="2c3b9-712">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-712">Boolean</span></span>|<span data-ttu-id="2c3b9-713">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-713">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="2c3b9-714">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="2c3b9-714">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="2c3b9-715">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-715">Boolean</span></span>|<span data-ttu-id="2c3b9-716">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-716">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="2c3b9-717">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-717">locationServicesBlocked</span></span>|<span data-ttu-id="2c3b9-718">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-718">Boolean</span></span>|<span data-ttu-id="2c3b9-719">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-719">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="2c3b9-720">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-720">microsoftAccountBlocked</span></span>|<span data-ttu-id="2c3b9-721">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-721">Boolean</span></span>|<span data-ttu-id="2c3b9-722">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-722">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="2c3b9-723">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="2c3b9-723">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="2c3b9-724">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-724">Boolean</span></span>|<span data-ttu-id="2c3b9-725">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-725">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="2c3b9-726">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-726">nfcBlocked</span></span>|<span data-ttu-id="2c3b9-727">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-727">Boolean</span></span>|<span data-ttu-id="2c3b9-728">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-728">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="2c3b9-729">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-729">resetProtectionModeBlocked</span></span>|<span data-ttu-id="2c3b9-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-730">Boolean</span></span>|<span data-ttu-id="2c3b9-731">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-731">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="2c3b9-732">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-732">screenCaptureBlocked</span></span>|<span data-ttu-id="2c3b9-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-733">Boolean</span></span>|<span data-ttu-id="2c3b9-734">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-734">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="2c3b9-735">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="2c3b9-735">storageBlockRemovableStorage</span></span>|<span data-ttu-id="2c3b9-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-736">Boolean</span></span>|<span data-ttu-id="2c3b9-737">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-737">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="2c3b9-738">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="2c3b9-738">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="2c3b9-739">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-739">Boolean</span></span>|<span data-ttu-id="2c3b9-740">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-740">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="2c3b9-741">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-741">usbBlocked</span></span>|<span data-ttu-id="2c3b9-742">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-742">Boolean</span></span>|<span data-ttu-id="2c3b9-743">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-743">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="2c3b9-744">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-744">voiceRecordingBlocked</span></span>|<span data-ttu-id="2c3b9-745">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-745">Boolean</span></span>|<span data-ttu-id="2c3b9-746">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-746">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="2c3b9-747">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="2c3b9-747">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="2c3b9-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-748">Boolean</span></span>|<span data-ttu-id="2c3b9-749">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-749">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="2c3b9-750">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-750">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="2c3b9-751">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-751">wiFiBlocked</span></span>|<span data-ttu-id="2c3b9-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-752">Boolean</span></span>|<span data-ttu-id="2c3b9-753">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-753">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="2c3b9-754">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c3b9-754">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="2c3b9-755">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-755">Boolean</span></span>|<span data-ttu-id="2c3b9-756">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-756">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="2c3b9-757">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="2c3b9-757">wiFiScanInterval</span></span>|<span data-ttu-id="2c3b9-758">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3b9-758">Int32</span></span>|<span data-ttu-id="2c3b9-759">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-759">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="2c3b9-760">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-760">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="2c3b9-761">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="2c3b9-761">Valid values 1 to 500</span></span>|
|<span data-ttu-id="2c3b9-762">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="2c3b9-762">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="2c3b9-763">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-763">Boolean</span></span>|<span data-ttu-id="2c3b9-764">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-764">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="2c3b9-765">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="2c3b9-765">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="2c3b9-766">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-766">Boolean</span></span>|<span data-ttu-id="2c3b9-767">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-767">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="2c3b9-768">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="2c3b9-768">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="2c3b9-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-769">Boolean</span></span>|<span data-ttu-id="2c3b9-770">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-770">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="2c3b9-771">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-771">windowsStoreBlocked</span></span>|<span data-ttu-id="2c3b9-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-772">Boolean</span></span>|<span data-ttu-id="2c3b9-773">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-773">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="2c3b9-774">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="2c3b9-774">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="2c3b9-775">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-775">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="2c3b9-776">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-776">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="2c3b9-777">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-777">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="2c3b9-778">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="2c3b9-778">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="2c3b9-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-779">Boolean</span></span>|<span data-ttu-id="2c3b9-780">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-780">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="2c3b9-781">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-781">developerUnlockSetting</span></span>|[<span data-ttu-id="2c3b9-782">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="2c3b9-782">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="2c3b9-783">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-783">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="2c3b9-784">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-784">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="2c3b9-785">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="2c3b9-785">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="2c3b9-786">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-786">Boolean</span></span>|<span data-ttu-id="2c3b9-787">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-787">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="2c3b9-788">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="2c3b9-788">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="2c3b9-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-789">Boolean</span></span>|<span data-ttu-id="2c3b9-790">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-790">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="2c3b9-791">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="2c3b9-791">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="2c3b9-792">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-792">Boolean</span></span>|<span data-ttu-id="2c3b9-793">指示是否启用“仅限专用应用商店”。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-793">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="2c3b9-794">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="2c3b9-794">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="2c3b9-795">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-795">Boolean</span></span>|<span data-ttu-id="2c3b9-796">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-796">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="2c3b9-797">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="2c3b9-797">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="2c3b9-798">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-798">Boolean</span></span>|<span data-ttu-id="2c3b9-799">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-799">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="2c3b9-800">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="2c3b9-800">gameDvrBlocked</span></span>|<span data-ttu-id="2c3b9-801">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-801">Boolean</span></span>|<span data-ttu-id="2c3b9-802">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-802">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="2c3b9-803">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="2c3b9-803">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="2c3b9-804">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-804">Boolean</span></span>|<span data-ttu-id="2c3b9-805">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-805">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="2c3b9-806">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="2c3b9-806">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="2c3b9-807">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-807">Boolean</span></span>|<span data-ttu-id="2c3b9-808">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-808">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="2c3b9-809">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="2c3b9-809">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="2c3b9-810">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-810">Boolean</span></span>|<span data-ttu-id="2c3b9-811">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-811">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="2c3b9-812">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="2c3b9-812">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="2c3b9-813">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-813">Boolean</span></span>|<span data-ttu-id="2c3b9-814">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-814">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="2c3b9-815">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="2c3b9-815">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="2c3b9-816">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3b9-816">Boolean</span></span>|<span data-ttu-id="2c3b9-817">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-817">Whether the device is required to connect to the network.</span></span>|



## <a name="response"></a><span data-ttu-id="2c3b9-818">响应</span><span class="sxs-lookup"><span data-stu-id="2c3b9-818">Response</span></span>
<span data-ttu-id="2c3b9-819">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-819">If successful, this method returns a `200 OK` response code and an updated [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c3b9-820">示例</span><span class="sxs-lookup"><span data-stu-id="2c3b9-820">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c3b9-821">请求</span><span class="sxs-lookup"><span data-stu-id="2c3b9-821">Request</span></span>
<span data-ttu-id="2c3b9-822">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-822">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="2c3b9-823">响应</span><span class="sxs-lookup"><span data-stu-id="2c3b9-823">Response</span></span>
<span data-ttu-id="2c3b9-p158">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c3b9-p158">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




