---
title: 更新 deviceManagementConfigurationSettingGroupCollectionDefinition
description: 更新 deviceManagementConfigurationSettingGroupCollectionDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5df45ef61eeee8e547c75491e21593e639fc3662
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241602"
---
# <a name="update-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="4f953-103">更新 deviceManagementConfigurationSettingGroupCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="4f953-103">Update deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="4f953-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f953-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f953-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f953-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f953-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f953-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f953-107">更新 [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4f953-107">Update the properties of a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f953-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4f953-108">Prerequisites</span></span>
<span data-ttu-id="4f953-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f953-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f953-111">Permission type</span></span>|<span data-ttu-id="4f953-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4f953-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f953-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f953-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f953-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f953-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f953-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f953-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f953-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f953-116">Not supported.</span></span>|
|<span data-ttu-id="4f953-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f953-117">Application</span></span>|<span data-ttu-id="4f953-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f953-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f953-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f953-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="4f953-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f953-120">Request headers</span></span>
|<span data-ttu-id="4f953-121">标头</span><span class="sxs-lookup"><span data-stu-id="4f953-121">Header</span></span>|<span data-ttu-id="4f953-122">值</span><span class="sxs-lookup"><span data-stu-id="4f953-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f953-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f953-123">Authorization</span></span>|<span data-ttu-id="4f953-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4f953-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f953-125">接受</span><span class="sxs-lookup"><span data-stu-id="4f953-125">Accept</span></span>|<span data-ttu-id="4f953-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f953-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f953-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f953-127">Request body</span></span>
<span data-ttu-id="4f953-128">在请求正文中，提供 [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f953-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

<span data-ttu-id="4f953-129">下表显示创建 [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4f953-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md).</span></span>

|<span data-ttu-id="4f953-130">属性</span><span class="sxs-lookup"><span data-stu-id="4f953-130">Property</span></span>|<span data-ttu-id="4f953-131">类型</span><span class="sxs-lookup"><span data-stu-id="4f953-131">Type</span></span>|<span data-ttu-id="4f953-132">描述</span><span class="sxs-lookup"><span data-stu-id="4f953-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f953-133">中期</span><span class="sxs-lookup"><span data-stu-id="4f953-133">applicability</span></span>|[<span data-ttu-id="4f953-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="4f953-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="4f953-135">详细介绍了哪些设备设置适用于继承自[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的设备</span><span class="sxs-lookup"><span data-stu-id="4f953-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="4f953-136">accessTypes</span></span>|[<span data-ttu-id="4f953-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="4f953-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="4f953-138">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的设置的读/写访问模式。</span><span class="sxs-lookup"><span data-stu-id="4f953-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="4f953-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="4f953-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="4f953-140">keywords</span><span class="sxs-lookup"><span data-stu-id="4f953-140">keywords</span></span>|<span data-ttu-id="4f953-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="4f953-141">String collection</span></span>|<span data-ttu-id="4f953-142">要在继承自[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)中搜索设置的标记</span><span class="sxs-lookup"><span data-stu-id="4f953-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="4f953-143">infoUrls</span></span>|<span data-ttu-id="4f953-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="4f953-144">String collection</span></span>|<span data-ttu-id="4f953-145">可从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的链接的详细信息列表。</span><span class="sxs-lookup"><span data-stu-id="4f953-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-146">重复</span><span class="sxs-lookup"><span data-stu-id="4f953-146">occurrence</span></span>|[<span data-ttu-id="4f953-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="4f953-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="4f953-148">指示是否需要设置或不继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4f953-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="4f953-149">baseUri</span></span>|<span data-ttu-id="4f953-150">String</span><span class="sxs-lookup"><span data-stu-id="4f953-150">String</span></span>|<span data-ttu-id="4f953-151">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的基本 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="4f953-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="4f953-152">offsetUri</span></span>|<span data-ttu-id="4f953-153">String</span><span class="sxs-lookup"><span data-stu-id="4f953-153">String</span></span>|<span data-ttu-id="4f953-154">从 Base 继承的[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)中偏移 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="4f953-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4f953-155">rootDefinitionId</span></span>|<span data-ttu-id="4f953-156">String</span><span class="sxs-lookup"><span data-stu-id="4f953-156">String</span></span>|<span data-ttu-id="4f953-157">根设置定义（如果设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="4f953-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="4f953-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4f953-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="4f953-159">categoryId</span></span>|<span data-ttu-id="4f953-160">String</span><span class="sxs-lookup"><span data-stu-id="4f953-160">String</span></span>|<span data-ttu-id="4f953-161">指定在指定的配置服务提供程序中配置设置的区域组 (CSP) 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4f953-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="4f953-162">settingUsage</span></span>|[<span data-ttu-id="4f953-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="4f953-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="4f953-164">设置类型，例如，从 [DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的配置和合规性。</span><span class="sxs-lookup"><span data-stu-id="4f953-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="4f953-165">可能的值是：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="4f953-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="4f953-166">id</span><span class="sxs-lookup"><span data-stu-id="4f953-166">id</span></span>|<span data-ttu-id="4f953-167">String</span><span class="sxs-lookup"><span data-stu-id="4f953-167">String</span></span>|<span data-ttu-id="4f953-168">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的标识符</span><span class="sxs-lookup"><span data-stu-id="4f953-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-169">description</span><span class="sxs-lookup"><span data-stu-id="4f953-169">description</span></span>|<span data-ttu-id="4f953-170">String</span><span class="sxs-lookup"><span data-stu-id="4f953-170">String</span></span>|<span data-ttu-id="4f953-171">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的说明</span><span class="sxs-lookup"><span data-stu-id="4f953-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-172">helpText</span><span class="sxs-lookup"><span data-stu-id="4f953-172">helpText</span></span>|<span data-ttu-id="4f953-173">String</span><span class="sxs-lookup"><span data-stu-id="4f953-173">String</span></span>|<span data-ttu-id="4f953-174">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的帮助文本</span><span class="sxs-lookup"><span data-stu-id="4f953-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-175">name</span><span class="sxs-lookup"><span data-stu-id="4f953-175">name</span></span>|<span data-ttu-id="4f953-176">String</span><span class="sxs-lookup"><span data-stu-id="4f953-176">String</span></span>|<span data-ttu-id="4f953-177">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的名称</span><span class="sxs-lookup"><span data-stu-id="4f953-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-178">displayName</span><span class="sxs-lookup"><span data-stu-id="4f953-178">displayName</span></span>|<span data-ttu-id="4f953-179">String</span><span class="sxs-lookup"><span data-stu-id="4f953-179">String</span></span>|<span data-ttu-id="4f953-180">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的显示名称</span><span class="sxs-lookup"><span data-stu-id="4f953-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-181">version</span><span class="sxs-lookup"><span data-stu-id="4f953-181">version</span></span>|<span data-ttu-id="4f953-182">String</span><span class="sxs-lookup"><span data-stu-id="4f953-182">String</span></span>|<span data-ttu-id="4f953-183">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项目版本</span><span class="sxs-lookup"><span data-stu-id="4f953-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4f953-184">childIds</span><span class="sxs-lookup"><span data-stu-id="4f953-184">childIds</span></span>|<span data-ttu-id="4f953-185">String 集合</span><span class="sxs-lookup"><span data-stu-id="4f953-185">String collection</span></span>|<span data-ttu-id="4f953-186">从[DeviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)继承的此组设置的从属子设置</span><span class="sxs-lookup"><span data-stu-id="4f953-186">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="4f953-187">dependentOn</span><span class="sxs-lookup"><span data-stu-id="4f953-187">dependentOn</span></span>|<span data-ttu-id="4f953-188">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f953-188">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="4f953-189">继承自[deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)的设置组的依赖项列表</span><span class="sxs-lookup"><span data-stu-id="4f953-189">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="4f953-190">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="4f953-190">dependedOnBy</span></span>|<span data-ttu-id="4f953-191">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f953-191">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="4f953-192">取决于从[DeviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)继承的此设置的子设置列表</span><span class="sxs-lookup"><span data-stu-id="4f953-192">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="4f953-193">maximumCount</span><span class="sxs-lookup"><span data-stu-id="4f953-193">maximumCount</span></span>|<span data-ttu-id="4f953-194">Int32</span><span class="sxs-lookup"><span data-stu-id="4f953-194">Int32</span></span>|<span data-ttu-id="4f953-195">集合中设置组计数的最大数目。</span><span class="sxs-lookup"><span data-stu-id="4f953-195">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="4f953-196">有效值为1至100</span><span class="sxs-lookup"><span data-stu-id="4f953-196">Valid values 1 to 100</span></span>|
|<span data-ttu-id="4f953-197">minimumCount</span><span class="sxs-lookup"><span data-stu-id="4f953-197">minimumCount</span></span>|<span data-ttu-id="4f953-198">Int32</span><span class="sxs-lookup"><span data-stu-id="4f953-198">Int32</span></span>|<span data-ttu-id="4f953-199">集合中设置组计数的最小数目。</span><span class="sxs-lookup"><span data-stu-id="4f953-199">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="4f953-200">有效值为1至100</span><span class="sxs-lookup"><span data-stu-id="4f953-200">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="4f953-201">响应</span><span class="sxs-lookup"><span data-stu-id="4f953-201">Response</span></span>
<span data-ttu-id="4f953-202">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f953-202">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f953-203">示例</span><span class="sxs-lookup"><span data-stu-id="4f953-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f953-204">请求</span><span class="sxs-lookup"><span data-stu-id="4f953-204">Request</span></span>
<span data-ttu-id="4f953-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f953-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1504

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="4f953-206">响应</span><span class="sxs-lookup"><span data-stu-id="4f953-206">Response</span></span>
<span data-ttu-id="4f953-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4f953-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1553

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
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
  "id": "739da194-a194-739d-94a1-9d7394a19d73",
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```




