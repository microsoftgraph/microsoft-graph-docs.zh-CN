---
title: 创建 deviceManagementConfigurationSettingDefinition
description: 创建新的 deviceManagementConfigurationSettingDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4730f642ba43b97211ab35053094e578956ac218
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146956"
---
# <a name="create-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="98a2a-103">创建 deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="98a2a-103">Create deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="98a2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98a2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98a2a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="98a2a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98a2a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98a2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98a2a-107">创建新的 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98a2a-107">Create a new [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98a2a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="98a2a-108">Prerequisites</span></span>
<span data-ttu-id="98a2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98a2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98a2a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="98a2a-111">Permission type</span></span>|<span data-ttu-id="98a2a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98a2a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98a2a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98a2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98a2a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98a2a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98a2a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98a2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98a2a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="98a2a-116">Not supported.</span></span>|
|<span data-ttu-id="98a2a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="98a2a-117">Application</span></span>|<span data-ttu-id="98a2a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98a2a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98a2a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98a2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="98a2a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="98a2a-120">Request headers</span></span>
|<span data-ttu-id="98a2a-121">标头</span><span class="sxs-lookup"><span data-stu-id="98a2a-121">Header</span></span>|<span data-ttu-id="98a2a-122">值</span><span class="sxs-lookup"><span data-stu-id="98a2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98a2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98a2a-123">Authorization</span></span>|<span data-ttu-id="98a2a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="98a2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98a2a-125">接受</span><span class="sxs-lookup"><span data-stu-id="98a2a-125">Accept</span></span>|<span data-ttu-id="98a2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98a2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98a2a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="98a2a-127">Request body</span></span>
<span data-ttu-id="98a2a-128">在请求正文中，提供 deviceManagementConfigurationSettingDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98a2a-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingDefinition object.</span></span>

<span data-ttu-id="98a2a-129">下表显示创建 deviceManagementConfigurationSettingDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="98a2a-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingDefinition.</span></span>

|<span data-ttu-id="98a2a-130">属性</span><span class="sxs-lookup"><span data-stu-id="98a2a-130">Property</span></span>|<span data-ttu-id="98a2a-131">类型</span><span class="sxs-lookup"><span data-stu-id="98a2a-131">Type</span></span>|<span data-ttu-id="98a2a-132">说明</span><span class="sxs-lookup"><span data-stu-id="98a2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98a2a-133">适用性</span><span class="sxs-lookup"><span data-stu-id="98a2a-133">applicability</span></span>|[<span data-ttu-id="98a2a-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="98a2a-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="98a2a-135">有关适用设备设置的详细信息</span><span class="sxs-lookup"><span data-stu-id="98a2a-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="98a2a-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="98a2a-136">accessTypes</span></span>|[<span data-ttu-id="98a2a-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="98a2a-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="98a2a-138">设置的读/写访问模式。</span><span class="sxs-lookup"><span data-stu-id="98a2a-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="98a2a-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="98a2a-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="98a2a-140">keywords</span><span class="sxs-lookup"><span data-stu-id="98a2a-140">keywords</span></span>|<span data-ttu-id="98a2a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="98a2a-141">String collection</span></span>|<span data-ttu-id="98a2a-142">要搜索设置的标记</span><span class="sxs-lookup"><span data-stu-id="98a2a-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="98a2a-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="98a2a-143">infoUrls</span></span>|<span data-ttu-id="98a2a-144">String collection</span><span class="sxs-lookup"><span data-stu-id="98a2a-144">String collection</span></span>|<span data-ttu-id="98a2a-145">可在以下链接列表中找到有关设置详细信息</span><span class="sxs-lookup"><span data-stu-id="98a2a-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="98a2a-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="98a2a-146">occurrence</span></span>|[<span data-ttu-id="98a2a-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="98a2a-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="98a2a-148">指示是否要求设置</span><span class="sxs-lookup"><span data-stu-id="98a2a-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="98a2a-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="98a2a-149">baseUri</span></span>|<span data-ttu-id="98a2a-150">String</span><span class="sxs-lookup"><span data-stu-id="98a2a-150">String</span></span>|<span data-ttu-id="98a2a-151">基本云解决方案提供商路径</span><span class="sxs-lookup"><span data-stu-id="98a2a-151">Base CSP Path</span></span>|
|<span data-ttu-id="98a2a-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="98a2a-152">offsetUri</span></span>|<span data-ttu-id="98a2a-153">String</span><span class="sxs-lookup"><span data-stu-id="98a2a-153">String</span></span>|<span data-ttu-id="98a2a-154">从基本位置偏移云解决方案提供商路径</span><span class="sxs-lookup"><span data-stu-id="98a2a-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="98a2a-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="98a2a-155">rootDefinitionId</span></span>|<span data-ttu-id="98a2a-156">String</span><span class="sxs-lookup"><span data-stu-id="98a2a-156">String</span></span>|<span data-ttu-id="98a2a-157">根设置定义（如果该设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="98a2a-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="98a2a-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="98a2a-158">categoryId</span></span>|<span data-ttu-id="98a2a-159">String</span><span class="sxs-lookup"><span data-stu-id="98a2a-159">String</span></span>|<span data-ttu-id="98a2a-160">指定在云解决方案提供商云解决方案提供商的指定配置服务提供程序中配置 (区域) </span><span class="sxs-lookup"><span data-stu-id="98a2a-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="98a2a-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="98a2a-161">settingUsage</span></span>|[<span data-ttu-id="98a2a-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="98a2a-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="98a2a-163">设置类型，例如配置和合规性。</span><span class="sxs-lookup"><span data-stu-id="98a2a-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="98a2a-164">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="98a2a-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="98a2a-165">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="98a2a-165">uxBehavior</span></span>|[<span data-ttu-id="98a2a-166">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="98a2a-166">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="98a2a-167">在 UX 中设置控件类型表示形式。</span><span class="sxs-lookup"><span data-stu-id="98a2a-167">Setting control type representation in the UX.</span></span> <span data-ttu-id="98a2a-168">可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。</span><span class="sxs-lookup"><span data-stu-id="98a2a-168">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="98a2a-169">visibility</span><span class="sxs-lookup"><span data-stu-id="98a2a-169">visibility</span></span>|[<span data-ttu-id="98a2a-170">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="98a2a-170">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="98a2a-171">将可见性范围设置为 UX。</span><span class="sxs-lookup"><span data-stu-id="98a2a-171">Setting visibility scope to UX.</span></span> <span data-ttu-id="98a2a-172">可取值为：`none`、`settingsCatalog`、`template`。</span><span class="sxs-lookup"><span data-stu-id="98a2a-172">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="98a2a-173">id</span><span class="sxs-lookup"><span data-stu-id="98a2a-173">id</span></span>|<span data-ttu-id="98a2a-174">String</span><span class="sxs-lookup"><span data-stu-id="98a2a-174">String</span></span>|<span data-ttu-id="98a2a-175">项的标识符</span><span class="sxs-lookup"><span data-stu-id="98a2a-175">Identifier for item</span></span>|
|<span data-ttu-id="98a2a-176">说明</span><span class="sxs-lookup"><span data-stu-id="98a2a-176">description</span></span>|<span data-ttu-id="98a2a-177">String</span><span class="sxs-lookup"><span data-stu-id="98a2a-177">String</span></span>|<span data-ttu-id="98a2a-178">项目说明</span><span class="sxs-lookup"><span data-stu-id="98a2a-178">Description of the item</span></span>|
|<span data-ttu-id="98a2a-179">helpText</span><span class="sxs-lookup"><span data-stu-id="98a2a-179">helpText</span></span>|<span data-ttu-id="98a2a-180">String</span><span class="sxs-lookup"><span data-stu-id="98a2a-180">String</span></span>|<span data-ttu-id="98a2a-181">项目的帮助文本</span><span class="sxs-lookup"><span data-stu-id="98a2a-181">Help text of the item</span></span>|
|<span data-ttu-id="98a2a-182">name</span><span class="sxs-lookup"><span data-stu-id="98a2a-182">name</span></span>|<span data-ttu-id="98a2a-183">String</span><span class="sxs-lookup"><span data-stu-id="98a2a-183">String</span></span>|<span data-ttu-id="98a2a-184">项目名称</span><span class="sxs-lookup"><span data-stu-id="98a2a-184">Name of the item</span></span>|
|<span data-ttu-id="98a2a-185">displayName</span><span class="sxs-lookup"><span data-stu-id="98a2a-185">displayName</span></span>|<span data-ttu-id="98a2a-186">String</span><span class="sxs-lookup"><span data-stu-id="98a2a-186">String</span></span>|<span data-ttu-id="98a2a-187">项目的显示名称</span><span class="sxs-lookup"><span data-stu-id="98a2a-187">Display name of the item</span></span>|
|<span data-ttu-id="98a2a-188">version</span><span class="sxs-lookup"><span data-stu-id="98a2a-188">version</span></span>|<span data-ttu-id="98a2a-189">String</span><span class="sxs-lookup"><span data-stu-id="98a2a-189">String</span></span>|<span data-ttu-id="98a2a-190">项目版本</span><span class="sxs-lookup"><span data-stu-id="98a2a-190">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="98a2a-191">响应</span><span class="sxs-lookup"><span data-stu-id="98a2a-191">Response</span></span>
<span data-ttu-id="98a2a-192">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98a2a-192">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98a2a-193">示例</span><span class="sxs-lookup"><span data-stu-id="98a2a-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="98a2a-194">请求</span><span class="sxs-lookup"><span data-stu-id="98a2a-194">Request</span></span>
<span data-ttu-id="98a2a-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="98a2a-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 1042

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
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="98a2a-196">响应</span><span class="sxs-lookup"><span data-stu-id="98a2a-196">Response</span></span>
<span data-ttu-id="98a2a-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="98a2a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1091

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
  "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```




