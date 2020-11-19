---
title: 创建 deviceManagementConfigurationSimpleSettingDefinition
description: 创建新的 deviceManagementConfigurationSimpleSettingDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6207e1e1dd2bc6eab6512a2fb909bb28b49aa45f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241576"
---
# <a name="create-devicemanagementconfigurationsimplesettingdefinition"></a><span data-ttu-id="ab642-103">创建 deviceManagementConfigurationSimpleSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="ab642-103">Create deviceManagementConfigurationSimpleSettingDefinition</span></span>

<span data-ttu-id="ab642-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab642-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab642-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ab642-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab642-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab642-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab642-107">创建新的 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ab642-107">Create a new [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab642-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ab642-108">Prerequisites</span></span>
<span data-ttu-id="ab642-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab642-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab642-111">Permission type</span></span>|<span data-ttu-id="ab642-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ab642-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab642-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab642-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab642-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab642-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab642-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab642-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab642-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab642-116">Not supported.</span></span>|
|<span data-ttu-id="ab642-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab642-117">Application</span></span>|<span data-ttu-id="ab642-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab642-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab642-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab642-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ab642-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab642-120">Request headers</span></span>
|<span data-ttu-id="ab642-121">标头</span><span class="sxs-lookup"><span data-stu-id="ab642-121">Header</span></span>|<span data-ttu-id="ab642-122">值</span><span class="sxs-lookup"><span data-stu-id="ab642-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab642-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab642-123">Authorization</span></span>|<span data-ttu-id="ab642-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ab642-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab642-125">接受</span><span class="sxs-lookup"><span data-stu-id="ab642-125">Accept</span></span>|<span data-ttu-id="ab642-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab642-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab642-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab642-127">Request body</span></span>
<span data-ttu-id="ab642-128">在请求正文中，提供 deviceManagementConfigurationSimpleSettingDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab642-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSimpleSettingDefinition object.</span></span>

<span data-ttu-id="ab642-129">下表显示创建 deviceManagementConfigurationSimpleSettingDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ab642-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSimpleSettingDefinition.</span></span>

|<span data-ttu-id="ab642-130">属性</span><span class="sxs-lookup"><span data-stu-id="ab642-130">Property</span></span>|<span data-ttu-id="ab642-131">类型</span><span class="sxs-lookup"><span data-stu-id="ab642-131">Type</span></span>|<span data-ttu-id="ab642-132">描述</span><span class="sxs-lookup"><span data-stu-id="ab642-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab642-133">中期</span><span class="sxs-lookup"><span data-stu-id="ab642-133">applicability</span></span>|[<span data-ttu-id="ab642-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="ab642-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="ab642-135">详细介绍了哪些设备设置适用于继承自[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的设备</span><span class="sxs-lookup"><span data-stu-id="ab642-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="ab642-136">accessTypes</span></span>|[<span data-ttu-id="ab642-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="ab642-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="ab642-138">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的设置的读/写访问模式。</span><span class="sxs-lookup"><span data-stu-id="ab642-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="ab642-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="ab642-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="ab642-140">keywords</span><span class="sxs-lookup"><span data-stu-id="ab642-140">keywords</span></span>|<span data-ttu-id="ab642-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="ab642-141">String collection</span></span>|<span data-ttu-id="ab642-142">要在继承自[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)中搜索设置的标记</span><span class="sxs-lookup"><span data-stu-id="ab642-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="ab642-143">infoUrls</span></span>|<span data-ttu-id="ab642-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="ab642-144">String collection</span></span>|<span data-ttu-id="ab642-145">可从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的链接的详细信息列表。</span><span class="sxs-lookup"><span data-stu-id="ab642-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-146">重复</span><span class="sxs-lookup"><span data-stu-id="ab642-146">occurrence</span></span>|[<span data-ttu-id="ab642-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="ab642-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="ab642-148">指示是否需要设置或不继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ab642-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="ab642-149">baseUri</span></span>|<span data-ttu-id="ab642-150">String</span><span class="sxs-lookup"><span data-stu-id="ab642-150">String</span></span>|<span data-ttu-id="ab642-151">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的基本 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="ab642-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="ab642-152">offsetUri</span></span>|<span data-ttu-id="ab642-153">String</span><span class="sxs-lookup"><span data-stu-id="ab642-153">String</span></span>|<span data-ttu-id="ab642-154">从 Base 继承的[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)中偏移 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="ab642-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ab642-155">rootDefinitionId</span></span>|<span data-ttu-id="ab642-156">String</span><span class="sxs-lookup"><span data-stu-id="ab642-156">String</span></span>|<span data-ttu-id="ab642-157">根设置定义（如果设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="ab642-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="ab642-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ab642-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="ab642-159">categoryId</span></span>|<span data-ttu-id="ab642-160">String</span><span class="sxs-lookup"><span data-stu-id="ab642-160">String</span></span>|<span data-ttu-id="ab642-161">指定在指定的配置服务提供程序中配置设置的区域组 (CSP) 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ab642-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="ab642-162">settingUsage</span></span>|[<span data-ttu-id="ab642-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="ab642-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="ab642-164">设置类型，例如，从 [DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的配置和合规性。</span><span class="sxs-lookup"><span data-stu-id="ab642-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="ab642-165">可能的值是：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="ab642-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="ab642-166">id</span><span class="sxs-lookup"><span data-stu-id="ab642-166">id</span></span>|<span data-ttu-id="ab642-167">String</span><span class="sxs-lookup"><span data-stu-id="ab642-167">String</span></span>|<span data-ttu-id="ab642-168">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的标识符</span><span class="sxs-lookup"><span data-stu-id="ab642-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-169">description</span><span class="sxs-lookup"><span data-stu-id="ab642-169">description</span></span>|<span data-ttu-id="ab642-170">String</span><span class="sxs-lookup"><span data-stu-id="ab642-170">String</span></span>|<span data-ttu-id="ab642-171">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的说明</span><span class="sxs-lookup"><span data-stu-id="ab642-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-172">helpText</span><span class="sxs-lookup"><span data-stu-id="ab642-172">helpText</span></span>|<span data-ttu-id="ab642-173">String</span><span class="sxs-lookup"><span data-stu-id="ab642-173">String</span></span>|<span data-ttu-id="ab642-174">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的帮助文本</span><span class="sxs-lookup"><span data-stu-id="ab642-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-175">name</span><span class="sxs-lookup"><span data-stu-id="ab642-175">name</span></span>|<span data-ttu-id="ab642-176">String</span><span class="sxs-lookup"><span data-stu-id="ab642-176">String</span></span>|<span data-ttu-id="ab642-177">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的名称</span><span class="sxs-lookup"><span data-stu-id="ab642-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-178">displayName</span><span class="sxs-lookup"><span data-stu-id="ab642-178">displayName</span></span>|<span data-ttu-id="ab642-179">String</span><span class="sxs-lookup"><span data-stu-id="ab642-179">String</span></span>|<span data-ttu-id="ab642-180">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的显示名称</span><span class="sxs-lookup"><span data-stu-id="ab642-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-181">version</span><span class="sxs-lookup"><span data-stu-id="ab642-181">version</span></span>|<span data-ttu-id="ab642-182">String</span><span class="sxs-lookup"><span data-stu-id="ab642-182">String</span></span>|<span data-ttu-id="ab642-183">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项目版本</span><span class="sxs-lookup"><span data-stu-id="ab642-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ab642-184">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="ab642-184">valueDefinition</span></span>|[<span data-ttu-id="ab642-185">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="ab642-185">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="ab642-186">此设置的值的定义</span><span class="sxs-lookup"><span data-stu-id="ab642-186">Definition of the value for this setting</span></span>|
|<span data-ttu-id="ab642-187">默认</span><span class="sxs-lookup"><span data-stu-id="ab642-187">defaultValue</span></span>|[<span data-ttu-id="ab642-188">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="ab642-188">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="ab642-189">此设置的默认设置值</span><span class="sxs-lookup"><span data-stu-id="ab642-189">Default setting value for this setting</span></span>|
|<span data-ttu-id="ab642-190">dependentOn</span><span class="sxs-lookup"><span data-stu-id="ab642-190">dependentOn</span></span>|<span data-ttu-id="ab642-191">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab642-191">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="ab642-192">此设置所依赖的父设置的列表</span><span class="sxs-lookup"><span data-stu-id="ab642-192">list of parent settings this setting is dependent on</span></span>|
|<span data-ttu-id="ab642-193">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="ab642-193">dependedOnBy</span></span>|<span data-ttu-id="ab642-194">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab642-194">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="ab642-195">依赖此设置的子设置的列表</span><span class="sxs-lookup"><span data-stu-id="ab642-195">list of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="ab642-196">响应</span><span class="sxs-lookup"><span data-stu-id="ab642-196">Response</span></span>
<span data-ttu-id="ab642-197">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ab642-197">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab642-198">示例</span><span class="sxs-lookup"><span data-stu-id="ab642-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab642-199">请求</span><span class="sxs-lookup"><span data-stu-id="ab642-199">Request</span></span>
<span data-ttu-id="ab642-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab642-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 9127

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingDefinition",
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
  "valueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueDefinition"
  },
  "defaultValue": {
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="ab642-201">响应</span><span class="sxs-lookup"><span data-stu-id="ab642-201">Response</span></span>
<span data-ttu-id="ab642-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab642-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9176

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingDefinition",
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
  "id": "30dc0613-0613-30dc-1306-dc301306dc30",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "valueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueDefinition"
  },
  "defaultValue": {
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
  ]
}
```




