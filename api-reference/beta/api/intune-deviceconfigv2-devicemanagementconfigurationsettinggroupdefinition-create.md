---
title: 创建 deviceManagementConfigurationSettingGroupDefinition
description: 创建新的 deviceManagementConfigurationSettingGroupDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c59ab6bd5a2aca7b4f6b11a2ad07ebe78ba766d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241593"
---
# <a name="create-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="ba8e8-103">创建 deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="ba8e8-103">Create deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="ba8e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba8e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba8e8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba8e8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba8e8-107">创建新的 [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-107">Create a new [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba8e8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ba8e8-108">Prerequisites</span></span>
<span data-ttu-id="ba8e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba8e8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba8e8-111">Permission type</span></span>|<span data-ttu-id="ba8e8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ba8e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba8e8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba8e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba8e8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba8e8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba8e8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba8e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba8e8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-116">Not supported.</span></span>|
|<span data-ttu-id="ba8e8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba8e8-117">Application</span></span>|<span data-ttu-id="ba8e8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba8e8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba8e8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba8e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ba8e8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba8e8-120">Request headers</span></span>
|<span data-ttu-id="ba8e8-121">标头</span><span class="sxs-lookup"><span data-stu-id="ba8e8-121">Header</span></span>|<span data-ttu-id="ba8e8-122">值</span><span class="sxs-lookup"><span data-stu-id="ba8e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba8e8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba8e8-123">Authorization</span></span>|<span data-ttu-id="ba8e8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba8e8-125">接受</span><span class="sxs-lookup"><span data-stu-id="ba8e8-125">Accept</span></span>|<span data-ttu-id="ba8e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba8e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba8e8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba8e8-127">Request body</span></span>
<span data-ttu-id="ba8e8-128">在请求正文中，提供 deviceManagementConfigurationSettingGroupDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupDefinition object.</span></span>

<span data-ttu-id="ba8e8-129">下表显示创建 deviceManagementConfigurationSettingGroupDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupDefinition.</span></span>

|<span data-ttu-id="ba8e8-130">属性</span><span class="sxs-lookup"><span data-stu-id="ba8e8-130">Property</span></span>|<span data-ttu-id="ba8e8-131">类型</span><span class="sxs-lookup"><span data-stu-id="ba8e8-131">Type</span></span>|<span data-ttu-id="ba8e8-132">描述</span><span class="sxs-lookup"><span data-stu-id="ba8e8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba8e8-133">中期</span><span class="sxs-lookup"><span data-stu-id="ba8e8-133">applicability</span></span>|[<span data-ttu-id="ba8e8-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="ba8e8-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="ba8e8-135">详细介绍了哪些设备设置适用于继承自[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的设备</span><span class="sxs-lookup"><span data-stu-id="ba8e8-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="ba8e8-136">accessTypes</span></span>|[<span data-ttu-id="ba8e8-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="ba8e8-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="ba8e8-138">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的设置的读/写访问模式。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="ba8e8-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="ba8e8-140">keywords</span><span class="sxs-lookup"><span data-stu-id="ba8e8-140">keywords</span></span>|<span data-ttu-id="ba8e8-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="ba8e8-141">String collection</span></span>|<span data-ttu-id="ba8e8-142">要在继承自[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)中搜索设置的标记</span><span class="sxs-lookup"><span data-stu-id="ba8e8-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="ba8e8-143">infoUrls</span></span>|<span data-ttu-id="ba8e8-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="ba8e8-144">String collection</span></span>|<span data-ttu-id="ba8e8-145">可从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的链接的详细信息列表。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-146">重复</span><span class="sxs-lookup"><span data-stu-id="ba8e8-146">occurrence</span></span>|[<span data-ttu-id="ba8e8-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="ba8e8-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="ba8e8-148">指示是否需要设置或不继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ba8e8-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="ba8e8-149">baseUri</span></span>|<span data-ttu-id="ba8e8-150">String</span><span class="sxs-lookup"><span data-stu-id="ba8e8-150">String</span></span>|<span data-ttu-id="ba8e8-151">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的基本 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="ba8e8-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="ba8e8-152">offsetUri</span></span>|<span data-ttu-id="ba8e8-153">String</span><span class="sxs-lookup"><span data-stu-id="ba8e8-153">String</span></span>|<span data-ttu-id="ba8e8-154">从 Base 继承的[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)中偏移 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="ba8e8-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ba8e8-155">rootDefinitionId</span></span>|<span data-ttu-id="ba8e8-156">String</span><span class="sxs-lookup"><span data-stu-id="ba8e8-156">String</span></span>|<span data-ttu-id="ba8e8-157">根设置定义（如果设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="ba8e8-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ba8e8-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="ba8e8-159">categoryId</span></span>|<span data-ttu-id="ba8e8-160">String</span><span class="sxs-lookup"><span data-stu-id="ba8e8-160">String</span></span>|<span data-ttu-id="ba8e8-161">指定在指定的配置服务提供程序中配置设置的区域组 (CSP) 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ba8e8-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="ba8e8-162">settingUsage</span></span>|[<span data-ttu-id="ba8e8-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="ba8e8-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="ba8e8-164">设置类型，例如，从 [DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的配置和合规性。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="ba8e8-165">可能的值是：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="ba8e8-166">id</span><span class="sxs-lookup"><span data-stu-id="ba8e8-166">id</span></span>|<span data-ttu-id="ba8e8-167">String</span><span class="sxs-lookup"><span data-stu-id="ba8e8-167">String</span></span>|<span data-ttu-id="ba8e8-168">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的标识符</span><span class="sxs-lookup"><span data-stu-id="ba8e8-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-169">description</span><span class="sxs-lookup"><span data-stu-id="ba8e8-169">description</span></span>|<span data-ttu-id="ba8e8-170">String</span><span class="sxs-lookup"><span data-stu-id="ba8e8-170">String</span></span>|<span data-ttu-id="ba8e8-171">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的说明</span><span class="sxs-lookup"><span data-stu-id="ba8e8-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-172">helpText</span><span class="sxs-lookup"><span data-stu-id="ba8e8-172">helpText</span></span>|<span data-ttu-id="ba8e8-173">String</span><span class="sxs-lookup"><span data-stu-id="ba8e8-173">String</span></span>|<span data-ttu-id="ba8e8-174">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的帮助文本</span><span class="sxs-lookup"><span data-stu-id="ba8e8-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-175">name</span><span class="sxs-lookup"><span data-stu-id="ba8e8-175">name</span></span>|<span data-ttu-id="ba8e8-176">String</span><span class="sxs-lookup"><span data-stu-id="ba8e8-176">String</span></span>|<span data-ttu-id="ba8e8-177">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的名称</span><span class="sxs-lookup"><span data-stu-id="ba8e8-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-178">displayName</span><span class="sxs-lookup"><span data-stu-id="ba8e8-178">displayName</span></span>|<span data-ttu-id="ba8e8-179">String</span><span class="sxs-lookup"><span data-stu-id="ba8e8-179">String</span></span>|<span data-ttu-id="ba8e8-180">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的显示名称</span><span class="sxs-lookup"><span data-stu-id="ba8e8-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-181">version</span><span class="sxs-lookup"><span data-stu-id="ba8e8-181">version</span></span>|<span data-ttu-id="ba8e8-182">String</span><span class="sxs-lookup"><span data-stu-id="ba8e8-182">String</span></span>|<span data-ttu-id="ba8e8-183">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项目版本</span><span class="sxs-lookup"><span data-stu-id="ba8e8-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ba8e8-184">childIds</span><span class="sxs-lookup"><span data-stu-id="ba8e8-184">childIds</span></span>|<span data-ttu-id="ba8e8-185">String 集合</span><span class="sxs-lookup"><span data-stu-id="ba8e8-185">String collection</span></span>|<span data-ttu-id="ba8e8-186">此组设置的从属子设置</span><span class="sxs-lookup"><span data-stu-id="ba8e8-186">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="ba8e8-187">dependentOn</span><span class="sxs-lookup"><span data-stu-id="ba8e8-187">dependentOn</span></span>|<span data-ttu-id="ba8e8-188">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ba8e8-188">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="ba8e8-189">设置组的依赖项列表</span><span class="sxs-lookup"><span data-stu-id="ba8e8-189">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="ba8e8-190">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="ba8e8-190">dependedOnBy</span></span>|<span data-ttu-id="ba8e8-191">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ba8e8-191">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="ba8e8-192">依赖此设置的子设置的列表</span><span class="sxs-lookup"><span data-stu-id="ba8e8-192">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="ba8e8-193">响应</span><span class="sxs-lookup"><span data-stu-id="ba8e8-193">Response</span></span>
<span data-ttu-id="ba8e8-194">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-194">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba8e8-195">示例</span><span class="sxs-lookup"><span data-stu-id="ba8e8-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba8e8-196">请求</span><span class="sxs-lookup"><span data-stu-id="ba8e8-196">Request</span></span>
<span data-ttu-id="ba8e8-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 1448

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
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
  "childIds": [
    "Child Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="ba8e8-198">响应</span><span class="sxs-lookup"><span data-stu-id="ba8e8-198">Response</span></span>
<span data-ttu-id="ba8e8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ba8e8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1497

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
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
  "id": "95dc9604-9604-95dc-0496-dc950496dc95",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "childIds": [
    "Child Ids value"
  ],
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




