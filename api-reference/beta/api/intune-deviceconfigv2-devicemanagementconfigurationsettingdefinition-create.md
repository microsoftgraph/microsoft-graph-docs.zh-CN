---
title: 创建 deviceManagementConfigurationSettingDefinition
description: 创建新的 deviceManagementConfigurationSettingDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c421989d170e99f2ce06aa86f5c856afdbcdcae
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665208"
---
# <a name="create-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="6ab61-103">创建 deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="6ab61-103">Create deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="6ab61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ab61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ab61-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ab61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ab61-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ab61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ab61-107">创建新的 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ab61-107">Create a new [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ab61-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6ab61-108">Prerequisites</span></span>
<span data-ttu-id="6ab61-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ab61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ab61-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ab61-111">Permission type</span></span>|<span data-ttu-id="6ab61-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ab61-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ab61-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ab61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ab61-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ab61-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ab61-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ab61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ab61-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ab61-116">Not supported.</span></span>|
|<span data-ttu-id="6ab61-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ab61-117">Application</span></span>|<span data-ttu-id="6ab61-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ab61-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ab61-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ab61-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusableSettings
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
POST /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="6ab61-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ab61-120">Request headers</span></span>
|<span data-ttu-id="6ab61-121">标头</span><span class="sxs-lookup"><span data-stu-id="6ab61-121">Header</span></span>|<span data-ttu-id="6ab61-122">值</span><span class="sxs-lookup"><span data-stu-id="6ab61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ab61-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ab61-123">Authorization</span></span>|<span data-ttu-id="6ab61-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6ab61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ab61-125">接受</span><span class="sxs-lookup"><span data-stu-id="6ab61-125">Accept</span></span>|<span data-ttu-id="6ab61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ab61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ab61-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ab61-127">Request body</span></span>
<span data-ttu-id="6ab61-128">在请求正文中，提供 deviceManagementConfigurationSettingDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ab61-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingDefinition object.</span></span>

<span data-ttu-id="6ab61-129">下表显示创建 deviceManagementConfigurationSettingDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6ab61-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingDefinition.</span></span>

|<span data-ttu-id="6ab61-130">属性</span><span class="sxs-lookup"><span data-stu-id="6ab61-130">Property</span></span>|<span data-ttu-id="6ab61-131">类型</span><span class="sxs-lookup"><span data-stu-id="6ab61-131">Type</span></span>|<span data-ttu-id="6ab61-132">说明</span><span class="sxs-lookup"><span data-stu-id="6ab61-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ab61-133">适用性</span><span class="sxs-lookup"><span data-stu-id="6ab61-133">applicability</span></span>|[<span data-ttu-id="6ab61-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="6ab61-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="6ab61-135">有关适用设备设置的详细信息</span><span class="sxs-lookup"><span data-stu-id="6ab61-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="6ab61-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="6ab61-136">accessTypes</span></span>|[<span data-ttu-id="6ab61-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="6ab61-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="6ab61-138">设置的读/写访问模式。</span><span class="sxs-lookup"><span data-stu-id="6ab61-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="6ab61-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="6ab61-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="6ab61-140">keywords</span><span class="sxs-lookup"><span data-stu-id="6ab61-140">keywords</span></span>|<span data-ttu-id="6ab61-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6ab61-141">String collection</span></span>|<span data-ttu-id="6ab61-142">要搜索设置的标记</span><span class="sxs-lookup"><span data-stu-id="6ab61-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="6ab61-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="6ab61-143">infoUrls</span></span>|<span data-ttu-id="6ab61-144">String collection</span><span class="sxs-lookup"><span data-stu-id="6ab61-144">String collection</span></span>|<span data-ttu-id="6ab61-145">可在以下链接列表中找到有关设置详细信息</span><span class="sxs-lookup"><span data-stu-id="6ab61-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="6ab61-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="6ab61-146">occurrence</span></span>|[<span data-ttu-id="6ab61-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="6ab61-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="6ab61-148">指示是否要求设置</span><span class="sxs-lookup"><span data-stu-id="6ab61-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="6ab61-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="6ab61-149">baseUri</span></span>|<span data-ttu-id="6ab61-150">String</span><span class="sxs-lookup"><span data-stu-id="6ab61-150">String</span></span>|<span data-ttu-id="6ab61-151">基本云解决方案提供商路径</span><span class="sxs-lookup"><span data-stu-id="6ab61-151">Base CSP Path</span></span>|
|<span data-ttu-id="6ab61-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="6ab61-152">offsetUri</span></span>|<span data-ttu-id="6ab61-153">String</span><span class="sxs-lookup"><span data-stu-id="6ab61-153">String</span></span>|<span data-ttu-id="6ab61-154">从基本位置偏移云解决方案提供商路径</span><span class="sxs-lookup"><span data-stu-id="6ab61-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="6ab61-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="6ab61-155">rootDefinitionId</span></span>|<span data-ttu-id="6ab61-156">String</span><span class="sxs-lookup"><span data-stu-id="6ab61-156">String</span></span>|<span data-ttu-id="6ab61-157">根设置定义（如果该设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="6ab61-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="6ab61-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="6ab61-158">categoryId</span></span>|<span data-ttu-id="6ab61-159">String</span><span class="sxs-lookup"><span data-stu-id="6ab61-159">String</span></span>|<span data-ttu-id="6ab61-160">指定在云解决方案提供商云解决方案提供商的指定配置服务提供程序中配置 (区域) </span><span class="sxs-lookup"><span data-stu-id="6ab61-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="6ab61-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="6ab61-161">settingUsage</span></span>|[<span data-ttu-id="6ab61-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="6ab61-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="6ab61-163">设置类型，例如配置和合规性。</span><span class="sxs-lookup"><span data-stu-id="6ab61-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="6ab61-164">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="6ab61-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="6ab61-165">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="6ab61-165">uxBehavior</span></span>|[<span data-ttu-id="6ab61-166">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="6ab61-166">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="6ab61-167">在 UX 中设置控件类型表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ab61-167">Setting control type representation in the UX.</span></span> <span data-ttu-id="6ab61-168">可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。</span><span class="sxs-lookup"><span data-stu-id="6ab61-168">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="6ab61-169">visibility</span><span class="sxs-lookup"><span data-stu-id="6ab61-169">visibility</span></span>|[<span data-ttu-id="6ab61-170">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="6ab61-170">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="6ab61-171">将可见性范围设置为 UX。</span><span class="sxs-lookup"><span data-stu-id="6ab61-171">Setting visibility scope to UX.</span></span> <span data-ttu-id="6ab61-172">可取值为：`none`、`settingsCatalog`、`template`。</span><span class="sxs-lookup"><span data-stu-id="6ab61-172">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="6ab61-173">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="6ab61-173">referredSettingInformationList</span></span>|<span data-ttu-id="6ab61-174">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6ab61-174">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="6ab61-175">引用的设置信息的列表。</span><span class="sxs-lookup"><span data-stu-id="6ab61-175">List of referred setting information.</span></span>|
|<span data-ttu-id="6ab61-176">id</span><span class="sxs-lookup"><span data-stu-id="6ab61-176">id</span></span>|<span data-ttu-id="6ab61-177">String</span><span class="sxs-lookup"><span data-stu-id="6ab61-177">String</span></span>|<span data-ttu-id="6ab61-178">项的标识符</span><span class="sxs-lookup"><span data-stu-id="6ab61-178">Identifier for item</span></span>|
|<span data-ttu-id="6ab61-179">说明</span><span class="sxs-lookup"><span data-stu-id="6ab61-179">description</span></span>|<span data-ttu-id="6ab61-180">String</span><span class="sxs-lookup"><span data-stu-id="6ab61-180">String</span></span>|<span data-ttu-id="6ab61-181">项目说明</span><span class="sxs-lookup"><span data-stu-id="6ab61-181">Description of the item</span></span>|
|<span data-ttu-id="6ab61-182">helpText</span><span class="sxs-lookup"><span data-stu-id="6ab61-182">helpText</span></span>|<span data-ttu-id="6ab61-183">String</span><span class="sxs-lookup"><span data-stu-id="6ab61-183">String</span></span>|<span data-ttu-id="6ab61-184">项目的帮助文本</span><span class="sxs-lookup"><span data-stu-id="6ab61-184">Help text of the item</span></span>|
|<span data-ttu-id="6ab61-185">name</span><span class="sxs-lookup"><span data-stu-id="6ab61-185">name</span></span>|<span data-ttu-id="6ab61-186">String</span><span class="sxs-lookup"><span data-stu-id="6ab61-186">String</span></span>|<span data-ttu-id="6ab61-187">项目名称</span><span class="sxs-lookup"><span data-stu-id="6ab61-187">Name of the item</span></span>|
|<span data-ttu-id="6ab61-188">displayName</span><span class="sxs-lookup"><span data-stu-id="6ab61-188">displayName</span></span>|<span data-ttu-id="6ab61-189">String</span><span class="sxs-lookup"><span data-stu-id="6ab61-189">String</span></span>|<span data-ttu-id="6ab61-190">项目的显示名称</span><span class="sxs-lookup"><span data-stu-id="6ab61-190">Display name of the item</span></span>|
|<span data-ttu-id="6ab61-191">version</span><span class="sxs-lookup"><span data-stu-id="6ab61-191">version</span></span>|<span data-ttu-id="6ab61-192">String</span><span class="sxs-lookup"><span data-stu-id="6ab61-192">String</span></span>|<span data-ttu-id="6ab61-193">项目版本</span><span class="sxs-lookup"><span data-stu-id="6ab61-193">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="6ab61-194">响应</span><span class="sxs-lookup"><span data-stu-id="6ab61-194">Response</span></span>
<span data-ttu-id="6ab61-195">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ab61-195">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ab61-196">示例</span><span class="sxs-lookup"><span data-stu-id="6ab61-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ab61-197">请求</span><span class="sxs-lookup"><span data-stu-id="6ab61-197">Request</span></span>
<span data-ttu-id="6ab61-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ab61-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusableSettings
Content-type: application/json
Content-length: 1258

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "macOS",
    "deviceMode": "kiosk",
    "technologies": "mdm"
  },
  "accessTypes": "add",
  "keywords": [
    "Keywords value"
  ],
  "infoUrls": [
    "Info Urls value"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 3,
    "maxDeviceOccurrence": 3
  },
  "baseUri": "Base Uri value",
  "offsetUri": "Offset Uri value",
  "rootDefinitionId": "Root Definition Id value",
  "categoryId": "Category Id value",
  "settingUsage": "configuration",
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="6ab61-199">响应</span><span class="sxs-lookup"><span data-stu-id="6ab61-199">Response</span></span>
<span data-ttu-id="6ab61-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ab61-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1307

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "macOS",
    "deviceMode": "kiosk",
    "technologies": "mdm"
  },
  "accessTypes": "add",
  "keywords": [
    "Keywords value"
  ],
  "infoUrls": [
    "Info Urls value"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 3,
    "maxDeviceOccurrence": 3
  },
  "baseUri": "Base Uri value",
  "offsetUri": "Offset Uri value",
  "rootDefinitionId": "Root Definition Id value",
  "categoryId": "Category Id value",
  "settingUsage": "configuration",
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
  "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```




