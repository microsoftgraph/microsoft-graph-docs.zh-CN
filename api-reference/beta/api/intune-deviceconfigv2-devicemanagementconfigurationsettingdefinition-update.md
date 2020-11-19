---
title: 更新 deviceManagementConfigurationSettingDefinition
description: 更新 deviceManagementConfigurationSettingDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb49bbd90b7c952deba932e0bbd1946f7bfc6ede
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241607"
---
# <a name="update-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="fb11c-103">更新 deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="fb11c-103">Update deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="fb11c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb11c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb11c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fb11c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb11c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb11c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb11c-107">更新 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fb11c-107">Update the properties of a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb11c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb11c-108">Prerequisites</span></span>
<span data-ttu-id="fb11c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb11c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb11c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb11c-111">Permission type</span></span>|<span data-ttu-id="fb11c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fb11c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb11c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb11c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb11c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb11c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb11c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb11c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb11c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb11c-116">Not supported.</span></span>|
|<span data-ttu-id="fb11c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb11c-117">Application</span></span>|<span data-ttu-id="fb11c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb11c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb11c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb11c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="fb11c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb11c-120">Request headers</span></span>
|<span data-ttu-id="fb11c-121">标头</span><span class="sxs-lookup"><span data-stu-id="fb11c-121">Header</span></span>|<span data-ttu-id="fb11c-122">值</span><span class="sxs-lookup"><span data-stu-id="fb11c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb11c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb11c-123">Authorization</span></span>|<span data-ttu-id="fb11c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb11c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb11c-125">接受</span><span class="sxs-lookup"><span data-stu-id="fb11c-125">Accept</span></span>|<span data-ttu-id="fb11c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb11c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb11c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb11c-127">Request body</span></span>
<span data-ttu-id="fb11c-128">在请求正文中，提供 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb11c-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

<span data-ttu-id="fb11c-129">下表显示创建 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fb11c-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span>

|<span data-ttu-id="fb11c-130">属性</span><span class="sxs-lookup"><span data-stu-id="fb11c-130">Property</span></span>|<span data-ttu-id="fb11c-131">类型</span><span class="sxs-lookup"><span data-stu-id="fb11c-131">Type</span></span>|<span data-ttu-id="fb11c-132">描述</span><span class="sxs-lookup"><span data-stu-id="fb11c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb11c-133">中期</span><span class="sxs-lookup"><span data-stu-id="fb11c-133">applicability</span></span>|[<span data-ttu-id="fb11c-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="fb11c-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="fb11c-135">详细介绍了适用于哪些设备设置</span><span class="sxs-lookup"><span data-stu-id="fb11c-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="fb11c-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="fb11c-136">accessTypes</span></span>|[<span data-ttu-id="fb11c-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="fb11c-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="fb11c-138">设置的读/写访问模式。</span><span class="sxs-lookup"><span data-stu-id="fb11c-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="fb11c-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="fb11c-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="fb11c-140">keywords</span><span class="sxs-lookup"><span data-stu-id="fb11c-140">keywords</span></span>|<span data-ttu-id="fb11c-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="fb11c-141">String collection</span></span>|<span data-ttu-id="fb11c-142">要在其上搜索设置的标记</span><span class="sxs-lookup"><span data-stu-id="fb11c-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="fb11c-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="fb11c-143">infoUrls</span></span>|<span data-ttu-id="fb11c-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="fb11c-144">String collection</span></span>|<span data-ttu-id="fb11c-145">可以在上找到有关此设置的详细信息的链接列表。</span><span class="sxs-lookup"><span data-stu-id="fb11c-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="fb11c-146">重复</span><span class="sxs-lookup"><span data-stu-id="fb11c-146">occurrence</span></span>|[<span data-ttu-id="fb11c-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="fb11c-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="fb11c-148">指示是否需要设置</span><span class="sxs-lookup"><span data-stu-id="fb11c-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="fb11c-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="fb11c-149">baseUri</span></span>|<span data-ttu-id="fb11c-150">String</span><span class="sxs-lookup"><span data-stu-id="fb11c-150">String</span></span>|<span data-ttu-id="fb11c-151">基本 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="fb11c-151">Base CSP Path</span></span>|
|<span data-ttu-id="fb11c-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="fb11c-152">offsetUri</span></span>|<span data-ttu-id="fb11c-153">String</span><span class="sxs-lookup"><span data-stu-id="fb11c-153">String</span></span>|<span data-ttu-id="fb11c-154">从 Base 中偏移 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="fb11c-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="fb11c-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fb11c-155">rootDefinitionId</span></span>|<span data-ttu-id="fb11c-156">String</span><span class="sxs-lookup"><span data-stu-id="fb11c-156">String</span></span>|<span data-ttu-id="fb11c-157">根设置定义（如果设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="fb11c-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="fb11c-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="fb11c-158">categoryId</span></span>|<span data-ttu-id="fb11c-159">String</span><span class="sxs-lookup"><span data-stu-id="fb11c-159">String</span></span>|<span data-ttu-id="fb11c-160">指定在指定的 configuration service 提供程序中配置设置所使用的区域组 (CSP) </span><span class="sxs-lookup"><span data-stu-id="fb11c-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="fb11c-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="fb11c-161">settingUsage</span></span>|[<span data-ttu-id="fb11c-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="fb11c-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="fb11c-163">设置类型，例如，配置和合规性。</span><span class="sxs-lookup"><span data-stu-id="fb11c-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="fb11c-164">可能的值是：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="fb11c-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="fb11c-165">id</span><span class="sxs-lookup"><span data-stu-id="fb11c-165">id</span></span>|<span data-ttu-id="fb11c-166">String</span><span class="sxs-lookup"><span data-stu-id="fb11c-166">String</span></span>|<span data-ttu-id="fb11c-167">项的标识符</span><span class="sxs-lookup"><span data-stu-id="fb11c-167">Identifier for item</span></span>|
|<span data-ttu-id="fb11c-168">description</span><span class="sxs-lookup"><span data-stu-id="fb11c-168">description</span></span>|<span data-ttu-id="fb11c-169">String</span><span class="sxs-lookup"><span data-stu-id="fb11c-169">String</span></span>|<span data-ttu-id="fb11c-170">项目的说明</span><span class="sxs-lookup"><span data-stu-id="fb11c-170">Description of the item</span></span>|
|<span data-ttu-id="fb11c-171">helpText</span><span class="sxs-lookup"><span data-stu-id="fb11c-171">helpText</span></span>|<span data-ttu-id="fb11c-172">String</span><span class="sxs-lookup"><span data-stu-id="fb11c-172">String</span></span>|<span data-ttu-id="fb11c-173">项目的帮助文本</span><span class="sxs-lookup"><span data-stu-id="fb11c-173">Help text of the item</span></span>|
|<span data-ttu-id="fb11c-174">name</span><span class="sxs-lookup"><span data-stu-id="fb11c-174">name</span></span>|<span data-ttu-id="fb11c-175">String</span><span class="sxs-lookup"><span data-stu-id="fb11c-175">String</span></span>|<span data-ttu-id="fb11c-176">项目的名称</span><span class="sxs-lookup"><span data-stu-id="fb11c-176">Name of the item</span></span>|
|<span data-ttu-id="fb11c-177">displayName</span><span class="sxs-lookup"><span data-stu-id="fb11c-177">displayName</span></span>|<span data-ttu-id="fb11c-178">String</span><span class="sxs-lookup"><span data-stu-id="fb11c-178">String</span></span>|<span data-ttu-id="fb11c-179">项目的显示名称</span><span class="sxs-lookup"><span data-stu-id="fb11c-179">Display name of the item</span></span>|
|<span data-ttu-id="fb11c-180">version</span><span class="sxs-lookup"><span data-stu-id="fb11c-180">version</span></span>|<span data-ttu-id="fb11c-181">String</span><span class="sxs-lookup"><span data-stu-id="fb11c-181">String</span></span>|<span data-ttu-id="fb11c-182">项目版本</span><span class="sxs-lookup"><span data-stu-id="fb11c-182">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="fb11c-183">响应</span><span class="sxs-lookup"><span data-stu-id="fb11c-183">Response</span></span>
<span data-ttu-id="fb11c-184">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb11c-184">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb11c-185">示例</span><span class="sxs-lookup"><span data-stu-id="fb11c-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb11c-186">请求</span><span class="sxs-lookup"><span data-stu-id="fb11c-186">Request</span></span>
<span data-ttu-id="fb11c-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb11c-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 977

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
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="fb11c-188">响应</span><span class="sxs-lookup"><span data-stu-id="fb11c-188">Response</span></span>
<span data-ttu-id="fb11c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb11c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1026

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
  "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```




