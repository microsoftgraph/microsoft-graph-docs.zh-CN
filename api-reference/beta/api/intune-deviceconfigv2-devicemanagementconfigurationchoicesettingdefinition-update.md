---
title: 更新 deviceManagementConfigurationChoiceSettingDefinition
description: 更新 deviceManagementConfigurationChoiceSettingDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69fac11d560de22f9537592edeed8bc63b01d44f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241505"
---
# <a name="update-devicemanagementconfigurationchoicesettingdefinition"></a><span data-ttu-id="ff201-103">更新 deviceManagementConfigurationChoiceSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="ff201-103">Update deviceManagementConfigurationChoiceSettingDefinition</span></span>

<span data-ttu-id="ff201-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff201-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff201-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff201-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff201-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff201-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff201-107">更新 [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff201-107">Update the properties of a [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff201-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ff201-108">Prerequisites</span></span>
<span data-ttu-id="ff201-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff201-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff201-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff201-111">Permission type</span></span>|<span data-ttu-id="ff201-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ff201-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff201-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff201-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff201-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff201-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff201-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff201-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff201-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff201-116">Not supported.</span></span>|
|<span data-ttu-id="ff201-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff201-117">Application</span></span>|<span data-ttu-id="ff201-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff201-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff201-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff201-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="ff201-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff201-120">Request headers</span></span>
|<span data-ttu-id="ff201-121">标头</span><span class="sxs-lookup"><span data-stu-id="ff201-121">Header</span></span>|<span data-ttu-id="ff201-122">值</span><span class="sxs-lookup"><span data-stu-id="ff201-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff201-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff201-123">Authorization</span></span>|<span data-ttu-id="ff201-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ff201-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff201-125">接受</span><span class="sxs-lookup"><span data-stu-id="ff201-125">Accept</span></span>|<span data-ttu-id="ff201-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff201-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff201-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff201-127">Request body</span></span>
<span data-ttu-id="ff201-128">在请求正文中，提供 [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff201-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object.</span></span>

<span data-ttu-id="ff201-129">下表显示创建 [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ff201-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md).</span></span>

|<span data-ttu-id="ff201-130">属性</span><span class="sxs-lookup"><span data-stu-id="ff201-130">Property</span></span>|<span data-ttu-id="ff201-131">类型</span><span class="sxs-lookup"><span data-stu-id="ff201-131">Type</span></span>|<span data-ttu-id="ff201-132">说明</span><span class="sxs-lookup"><span data-stu-id="ff201-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff201-133">中期</span><span class="sxs-lookup"><span data-stu-id="ff201-133">applicability</span></span>|[<span data-ttu-id="ff201-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="ff201-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="ff201-135">详细介绍了哪些设备设置适用于继承自[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的设备</span><span class="sxs-lookup"><span data-stu-id="ff201-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="ff201-136">accessTypes</span></span>|[<span data-ttu-id="ff201-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="ff201-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="ff201-138">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的设置的读/写访问模式。</span><span class="sxs-lookup"><span data-stu-id="ff201-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="ff201-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="ff201-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="ff201-140">keywords</span><span class="sxs-lookup"><span data-stu-id="ff201-140">keywords</span></span>|<span data-ttu-id="ff201-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="ff201-141">String collection</span></span>|<span data-ttu-id="ff201-142">要在继承自[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)中搜索设置的标记</span><span class="sxs-lookup"><span data-stu-id="ff201-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="ff201-143">infoUrls</span></span>|<span data-ttu-id="ff201-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="ff201-144">String collection</span></span>|<span data-ttu-id="ff201-145">可从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的链接的详细信息列表。</span><span class="sxs-lookup"><span data-stu-id="ff201-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-146">重复</span><span class="sxs-lookup"><span data-stu-id="ff201-146">occurrence</span></span>|[<span data-ttu-id="ff201-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="ff201-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="ff201-148">指示是否需要设置或不继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff201-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="ff201-149">baseUri</span></span>|<span data-ttu-id="ff201-150">String</span><span class="sxs-lookup"><span data-stu-id="ff201-150">String</span></span>|<span data-ttu-id="ff201-151">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的基本 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="ff201-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="ff201-152">offsetUri</span></span>|<span data-ttu-id="ff201-153">String</span><span class="sxs-lookup"><span data-stu-id="ff201-153">String</span></span>|<span data-ttu-id="ff201-154">从 Base 继承的[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)中偏移 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="ff201-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ff201-155">rootDefinitionId</span></span>|<span data-ttu-id="ff201-156">String</span><span class="sxs-lookup"><span data-stu-id="ff201-156">String</span></span>|<span data-ttu-id="ff201-157">根设置定义（如果设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="ff201-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="ff201-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff201-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="ff201-159">categoryId</span></span>|<span data-ttu-id="ff201-160">String</span><span class="sxs-lookup"><span data-stu-id="ff201-160">String</span></span>|<span data-ttu-id="ff201-161">指定在指定的配置服务提供程序中配置设置的区域组 (CSP) 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff201-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="ff201-162">settingUsage</span></span>|[<span data-ttu-id="ff201-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="ff201-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="ff201-164">设置类型，例如，从 [DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的配置和合规性。</span><span class="sxs-lookup"><span data-stu-id="ff201-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="ff201-165">可能的值是：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="ff201-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="ff201-166">id</span><span class="sxs-lookup"><span data-stu-id="ff201-166">id</span></span>|<span data-ttu-id="ff201-167">String</span><span class="sxs-lookup"><span data-stu-id="ff201-167">String</span></span>|<span data-ttu-id="ff201-168">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的标识符</span><span class="sxs-lookup"><span data-stu-id="ff201-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-169">description</span><span class="sxs-lookup"><span data-stu-id="ff201-169">description</span></span>|<span data-ttu-id="ff201-170">String</span><span class="sxs-lookup"><span data-stu-id="ff201-170">String</span></span>|<span data-ttu-id="ff201-171">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的说明</span><span class="sxs-lookup"><span data-stu-id="ff201-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-172">helpText</span><span class="sxs-lookup"><span data-stu-id="ff201-172">helpText</span></span>|<span data-ttu-id="ff201-173">String</span><span class="sxs-lookup"><span data-stu-id="ff201-173">String</span></span>|<span data-ttu-id="ff201-174">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的帮助文本</span><span class="sxs-lookup"><span data-stu-id="ff201-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-175">name</span><span class="sxs-lookup"><span data-stu-id="ff201-175">name</span></span>|<span data-ttu-id="ff201-176">String</span><span class="sxs-lookup"><span data-stu-id="ff201-176">String</span></span>|<span data-ttu-id="ff201-177">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的名称</span><span class="sxs-lookup"><span data-stu-id="ff201-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-178">displayName</span><span class="sxs-lookup"><span data-stu-id="ff201-178">displayName</span></span>|<span data-ttu-id="ff201-179">String</span><span class="sxs-lookup"><span data-stu-id="ff201-179">String</span></span>|<span data-ttu-id="ff201-180">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的显示名称</span><span class="sxs-lookup"><span data-stu-id="ff201-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-181">version</span><span class="sxs-lookup"><span data-stu-id="ff201-181">version</span></span>|<span data-ttu-id="ff201-182">String</span><span class="sxs-lookup"><span data-stu-id="ff201-182">String</span></span>|<span data-ttu-id="ff201-183">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项目版本</span><span class="sxs-lookup"><span data-stu-id="ff201-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ff201-184">选项</span><span class="sxs-lookup"><span data-stu-id="ff201-184">options</span></span>|<span data-ttu-id="ff201-185">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff201-185">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) collection</span></span>|<span data-ttu-id="ff201-186">可选择的设置的选项</span><span class="sxs-lookup"><span data-stu-id="ff201-186">Options for the setting that can be selected</span></span>|
|<span data-ttu-id="ff201-187">defaultOptionId</span><span class="sxs-lookup"><span data-stu-id="ff201-187">defaultOptionId</span></span>|<span data-ttu-id="ff201-188">String</span><span class="sxs-lookup"><span data-stu-id="ff201-188">String</span></span>|<span data-ttu-id="ff201-189">选项设置的默认选项</span><span class="sxs-lookup"><span data-stu-id="ff201-189">Default option for choice setting</span></span>|



## <a name="response"></a><span data-ttu-id="ff201-190">响应</span><span class="sxs-lookup"><span data-stu-id="ff201-190">Response</span></span>
<span data-ttu-id="ff201-191">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff201-191">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff201-192">示例</span><span class="sxs-lookup"><span data-stu-id="ff201-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff201-193">请求</span><span class="sxs-lookup"><span data-stu-id="ff201-193">Request</span></span>
<span data-ttu-id="ff201-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff201-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 9877

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingDefinition",
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
  "version": "Version value",
  "options": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition",
      "optionValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
        "children": [
          {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
            "settingDefinitionId": "Setting Definition Id value",
            "choiceSettingValue": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
              "value": "Value value",
              "children": [
                {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                  "settingDefinitionId": "Setting Definition Id value",
                  "choiceSettingValue": {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                    "value": "Value value",
                    "children": [
                      {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                        "settingDefinitionId": "Setting Definition Id value",
                        "choiceSettingValue": {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                          "value": "Value value",
                          "children": [
                            {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                              "settingDefinitionId": "Setting Definition Id value",
                              "choiceSettingValue": {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                "value": "Value value",
                                "children": [
                                  {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                    "settingDefinitionId": "Setting Definition Id value",
                                    "choiceSettingValue": {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                      "value": "Value value",
                                      "children": [
                                        {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                          "settingDefinitionId": "Setting Definition Id value",
                                          "choiceSettingValue": {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                            "value": "Value value",
                                            "children": [
                                              {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                "settingDefinitionId": "Setting Definition Id value",
                                                "choiceSettingValue": {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                  "value": "Value value",
                                                  "children": [
                                                    {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                      "settingDefinitionId": "Setting Definition Id value",
                                                      "choiceSettingValue": {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                        "value": "Value value",
                                                        "children": [
                                                          {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                            "settingDefinitionId": "Setting Definition Id value",
                                                            "choiceSettingValue": {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                              "value": "Value value",
                                                              "children": [
                                                                {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                  "settingDefinitionId": "Setting Definition Id value",
                                                                  "choiceSettingValue": {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                    "value": "Value value",
                                                                    "children": [
                                                                      {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                        "settingDefinitionId": "Setting Definition Id value",
                                                                        "choiceSettingValue": {
                                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                          "value": "Value value",
                                                                          "children": null
                                                                        }
                                                                      }
                                                                    ]
                                                                  }
                                                                }
                                                              ]
                                                            }
                                                          }
                                                        ]
                                                      }
                                                    }
                                                  ]
                                                }
                                              }
                                            ]
                                          }
                                        }
                                      ]
                                    }
                                  }
                                ]
                              }
                            }
                          ]
                        }
                      }
                    ]
                  }
                }
              ]
            }
          }
        ]
      },
      "dependentOn": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
          "dependentOn": "Dependent On value",
          "parentSettingId": "Parent Setting Id value"
        }
      ],
      "dependedOnBy": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
          "dependedOnBy": "Depended On By value",
          "required": true
        }
      ],
      "itemId": "Item Id value",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value"
    }
  ],
  "defaultOptionId": "Default Option Id value"
}
```

### <a name="response"></a><span data-ttu-id="ff201-195">响应</span><span class="sxs-lookup"><span data-stu-id="ff201-195">Response</span></span>
<span data-ttu-id="ff201-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff201-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9926

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingDefinition",
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
  "id": "30b2258a-258a-30b2-8a25-b2308a25b230",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "options": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition",
      "optionValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
        "children": [
          {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
            "settingDefinitionId": "Setting Definition Id value",
            "choiceSettingValue": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
              "value": "Value value",
              "children": [
                {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                  "settingDefinitionId": "Setting Definition Id value",
                  "choiceSettingValue": {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                    "value": "Value value",
                    "children": [
                      {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                        "settingDefinitionId": "Setting Definition Id value",
                        "choiceSettingValue": {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                          "value": "Value value",
                          "children": [
                            {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                              "settingDefinitionId": "Setting Definition Id value",
                              "choiceSettingValue": {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                "value": "Value value",
                                "children": [
                                  {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                    "settingDefinitionId": "Setting Definition Id value",
                                    "choiceSettingValue": {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                      "value": "Value value",
                                      "children": [
                                        {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                          "settingDefinitionId": "Setting Definition Id value",
                                          "choiceSettingValue": {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                            "value": "Value value",
                                            "children": [
                                              {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                "settingDefinitionId": "Setting Definition Id value",
                                                "choiceSettingValue": {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                  "value": "Value value",
                                                  "children": [
                                                    {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                      "settingDefinitionId": "Setting Definition Id value",
                                                      "choiceSettingValue": {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                        "value": "Value value",
                                                        "children": [
                                                          {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                            "settingDefinitionId": "Setting Definition Id value",
                                                            "choiceSettingValue": {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                              "value": "Value value",
                                                              "children": [
                                                                {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                  "settingDefinitionId": "Setting Definition Id value",
                                                                  "choiceSettingValue": {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                    "value": "Value value",
                                                                    "children": [
                                                                      {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                        "settingDefinitionId": "Setting Definition Id value",
                                                                        "choiceSettingValue": {
                                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                          "value": "Value value",
                                                                          "children": null
                                                                        }
                                                                      }
                                                                    ]
                                                                  }
                                                                }
                                                              ]
                                                            }
                                                          }
                                                        ]
                                                      }
                                                    }
                                                  ]
                                                }
                                              }
                                            ]
                                          }
                                        }
                                      ]
                                    }
                                  }
                                ]
                              }
                            }
                          ]
                        }
                      }
                    ]
                  }
                }
              ]
            }
          }
        ]
      },
      "dependentOn": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
          "dependentOn": "Dependent On value",
          "parentSettingId": "Parent Setting Id value"
        }
      ],
      "dependedOnBy": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
          "dependedOnBy": "Depended On By value",
          "required": true
        }
      ],
      "itemId": "Item Id value",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value"
    }
  ],
  "defaultOptionId": "Default Option Id value"
}
```




