---
title: 创建 deviceManagementConfigurationSettingDefinition
description: 创建新的 deviceManagementConfigurationSettingDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8948ad0f1c4224a1febc0bbd84433c26674065b3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161093"
---
# <a name="create-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="b0c4d-103">创建 deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="b0c4d-103">Create deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="b0c4d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0c4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0c4d-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0c4d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0c4d-107">创建新的 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-107">Create a new [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0c4d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0c4d-108">Prerequisites</span></span>
<span data-ttu-id="b0c4d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0c4d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0c4d-111">Permission type</span></span>|<span data-ttu-id="b0c4d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b0c4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0c4d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0c4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0c4d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0c4d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0c4d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0c4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0c4d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-116">Not supported.</span></span>|
|<span data-ttu-id="b0c4d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0c4d-117">Application</span></span>|<span data-ttu-id="b0c4d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0c4d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0c4d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0c4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="b0c4d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0c4d-120">Request headers</span></span>
|<span data-ttu-id="b0c4d-121">标头</span><span class="sxs-lookup"><span data-stu-id="b0c4d-121">Header</span></span>|<span data-ttu-id="b0c4d-122">值</span><span class="sxs-lookup"><span data-stu-id="b0c4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0c4d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0c4d-123">Authorization</span></span>|<span data-ttu-id="b0c4d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0c4d-125">接受</span><span class="sxs-lookup"><span data-stu-id="b0c4d-125">Accept</span></span>|<span data-ttu-id="b0c4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0c4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0c4d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0c4d-127">Request body</span></span>
<span data-ttu-id="b0c4d-128">在请求正文中，提供 deviceManagementConfigurationSettingDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingDefinition object.</span></span>

<span data-ttu-id="b0c4d-129">下表显示创建 deviceManagementConfigurationSettingDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingDefinition.</span></span>

|<span data-ttu-id="b0c4d-130">属性</span><span class="sxs-lookup"><span data-stu-id="b0c4d-130">Property</span></span>|<span data-ttu-id="b0c4d-131">类型</span><span class="sxs-lookup"><span data-stu-id="b0c4d-131">Type</span></span>|<span data-ttu-id="b0c4d-132">说明</span><span class="sxs-lookup"><span data-stu-id="b0c4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0c4d-133">适用性</span><span class="sxs-lookup"><span data-stu-id="b0c4d-133">applicability</span></span>|[<span data-ttu-id="b0c4d-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="b0c4d-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="b0c4d-135">有关适用于哪些设备设置的详细信息</span><span class="sxs-lookup"><span data-stu-id="b0c4d-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="b0c4d-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="b0c4d-136">accessTypes</span></span>|[<span data-ttu-id="b0c4d-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="b0c4d-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="b0c4d-138">设置的读/写访问模式。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="b0c4d-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="b0c4d-140">keywords</span><span class="sxs-lookup"><span data-stu-id="b0c4d-140">keywords</span></span>|<span data-ttu-id="b0c4d-141">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b0c4d-141">String collection</span></span>|<span data-ttu-id="b0c4d-142">要搜索设置的标记</span><span class="sxs-lookup"><span data-stu-id="b0c4d-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="b0c4d-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="b0c4d-143">infoUrls</span></span>|<span data-ttu-id="b0c4d-144">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b0c4d-144">String collection</span></span>|<span data-ttu-id="b0c4d-145">可在以下链接列表中找到设置详细信息</span><span class="sxs-lookup"><span data-stu-id="b0c4d-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="b0c4d-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="b0c4d-146">occurrence</span></span>|[<span data-ttu-id="b0c4d-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="b0c4d-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="b0c4d-148">指示设置是否是必需的</span><span class="sxs-lookup"><span data-stu-id="b0c4d-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="b0c4d-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="b0c4d-149">baseUri</span></span>|<span data-ttu-id="b0c4d-150">String</span><span class="sxs-lookup"><span data-stu-id="b0c4d-150">String</span></span>|<span data-ttu-id="b0c4d-151">基本云解决方案提供商路径</span><span class="sxs-lookup"><span data-stu-id="b0c4d-151">Base CSP Path</span></span>|
|<span data-ttu-id="b0c4d-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="b0c4d-152">offsetUri</span></span>|<span data-ttu-id="b0c4d-153">String</span><span class="sxs-lookup"><span data-stu-id="b0c4d-153">String</span></span>|<span data-ttu-id="b0c4d-154">从基本偏移云解决方案提供商路径</span><span class="sxs-lookup"><span data-stu-id="b0c4d-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="b0c4d-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b0c4d-155">rootDefinitionId</span></span>|<span data-ttu-id="b0c4d-156">String</span><span class="sxs-lookup"><span data-stu-id="b0c4d-156">String</span></span>|<span data-ttu-id="b0c4d-157">根设置定义（如果该设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="b0c4d-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="b0c4d-158">categoryId</span></span>|<span data-ttu-id="b0c4d-159">String</span><span class="sxs-lookup"><span data-stu-id="b0c4d-159">String</span></span>|<span data-ttu-id="b0c4d-160">指定在云解决方案提供商云解决方案提供商的指定配置服务提供程序中配置 (区域) </span><span class="sxs-lookup"><span data-stu-id="b0c4d-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="b0c4d-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="b0c4d-161">settingUsage</span></span>|[<span data-ttu-id="b0c4d-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="b0c4d-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="b0c4d-163">设置类型，例如配置和合规性。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="b0c4d-164">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="b0c4d-165">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="b0c4d-165">uxBehavior</span></span>|[<span data-ttu-id="b0c4d-166">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="b0c4d-166">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="b0c4d-167">在 UX 中设置控件类型表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-167">Setting control type representation in the UX.</span></span> <span data-ttu-id="b0c4d-168">可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-168">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="b0c4d-169">id</span><span class="sxs-lookup"><span data-stu-id="b0c4d-169">id</span></span>|<span data-ttu-id="b0c4d-170">String</span><span class="sxs-lookup"><span data-stu-id="b0c4d-170">String</span></span>|<span data-ttu-id="b0c4d-171">项的标识符</span><span class="sxs-lookup"><span data-stu-id="b0c4d-171">Identifier for item</span></span>|
|<span data-ttu-id="b0c4d-172">说明</span><span class="sxs-lookup"><span data-stu-id="b0c4d-172">description</span></span>|<span data-ttu-id="b0c4d-173">String</span><span class="sxs-lookup"><span data-stu-id="b0c4d-173">String</span></span>|<span data-ttu-id="b0c4d-174">项目说明</span><span class="sxs-lookup"><span data-stu-id="b0c4d-174">Description of the item</span></span>|
|<span data-ttu-id="b0c4d-175">helpText</span><span class="sxs-lookup"><span data-stu-id="b0c4d-175">helpText</span></span>|<span data-ttu-id="b0c4d-176">String</span><span class="sxs-lookup"><span data-stu-id="b0c4d-176">String</span></span>|<span data-ttu-id="b0c4d-177">项目的帮助文本</span><span class="sxs-lookup"><span data-stu-id="b0c4d-177">Help text of the item</span></span>|
|<span data-ttu-id="b0c4d-178">名称</span><span class="sxs-lookup"><span data-stu-id="b0c4d-178">name</span></span>|<span data-ttu-id="b0c4d-179">String</span><span class="sxs-lookup"><span data-stu-id="b0c4d-179">String</span></span>|<span data-ttu-id="b0c4d-180">项目名称</span><span class="sxs-lookup"><span data-stu-id="b0c4d-180">Name of the item</span></span>|
|<span data-ttu-id="b0c4d-181">displayName</span><span class="sxs-lookup"><span data-stu-id="b0c4d-181">displayName</span></span>|<span data-ttu-id="b0c4d-182">String</span><span class="sxs-lookup"><span data-stu-id="b0c4d-182">String</span></span>|<span data-ttu-id="b0c4d-183">项目的显示名称</span><span class="sxs-lookup"><span data-stu-id="b0c4d-183">Display name of the item</span></span>|
|<span data-ttu-id="b0c4d-184">version</span><span class="sxs-lookup"><span data-stu-id="b0c4d-184">version</span></span>|<span data-ttu-id="b0c4d-185">String</span><span class="sxs-lookup"><span data-stu-id="b0c4d-185">String</span></span>|<span data-ttu-id="b0c4d-186">项目版本</span><span class="sxs-lookup"><span data-stu-id="b0c4d-186">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="b0c4d-187">响应</span><span class="sxs-lookup"><span data-stu-id="b0c4d-187">Response</span></span>
<span data-ttu-id="b0c4d-188">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-188">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0c4d-189">示例</span><span class="sxs-lookup"><span data-stu-id="b0c4d-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0c4d-190">请求</span><span class="sxs-lookup"><span data-stu-id="b0c4d-190">Request</span></span>
<span data-ttu-id="b0c4d-191">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 1006

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
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="b0c4d-192">响应</span><span class="sxs-lookup"><span data-stu-id="b0c4d-192">Response</span></span>
<span data-ttu-id="b0c4d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0c4d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1055

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
  "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```




