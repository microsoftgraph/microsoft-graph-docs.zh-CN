---
title: 更新 deviceManagementConfigurationSimpleSettingCollectionDefinition
description: 更新 deviceManagementConfigurationSimpleSettingCollectionDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f55e7a6437da546d0b762ed6fd329d833efeae4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241582"
---
# <a name="update-devicemanagementconfigurationsimplesettingcollectiondefinition"></a><span data-ttu-id="4de62-103">更新 deviceManagementConfigurationSimpleSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="4de62-103">Update deviceManagementConfigurationSimpleSettingCollectionDefinition</span></span>

<span data-ttu-id="4de62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4de62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4de62-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4de62-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4de62-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4de62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4de62-107">更新 [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4de62-107">Update the properties of a [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4de62-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4de62-108">Prerequisites</span></span>
<span data-ttu-id="4de62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4de62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4de62-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4de62-111">Permission type</span></span>|<span data-ttu-id="4de62-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4de62-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4de62-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4de62-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4de62-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de62-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4de62-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4de62-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4de62-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4de62-116">Not supported.</span></span>|
|<span data-ttu-id="4de62-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4de62-117">Application</span></span>|<span data-ttu-id="4de62-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de62-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4de62-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4de62-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="4de62-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4de62-120">Request headers</span></span>
|<span data-ttu-id="4de62-121">标头</span><span class="sxs-lookup"><span data-stu-id="4de62-121">Header</span></span>|<span data-ttu-id="4de62-122">值</span><span class="sxs-lookup"><span data-stu-id="4de62-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4de62-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4de62-123">Authorization</span></span>|<span data-ttu-id="4de62-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4de62-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4de62-125">接受</span><span class="sxs-lookup"><span data-stu-id="4de62-125">Accept</span></span>|<span data-ttu-id="4de62-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4de62-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4de62-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4de62-127">Request body</span></span>
<span data-ttu-id="4de62-128">在请求正文中，提供 [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4de62-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

<span data-ttu-id="4de62-129">下表显示创建 [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4de62-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md).</span></span>

|<span data-ttu-id="4de62-130">属性</span><span class="sxs-lookup"><span data-stu-id="4de62-130">Property</span></span>|<span data-ttu-id="4de62-131">类型</span><span class="sxs-lookup"><span data-stu-id="4de62-131">Type</span></span>|<span data-ttu-id="4de62-132">描述</span><span class="sxs-lookup"><span data-stu-id="4de62-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4de62-133">中期</span><span class="sxs-lookup"><span data-stu-id="4de62-133">applicability</span></span>|[<span data-ttu-id="4de62-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="4de62-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="4de62-135">详细介绍了哪些设备设置适用于继承自[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的设备</span><span class="sxs-lookup"><span data-stu-id="4de62-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="4de62-136">accessTypes</span></span>|[<span data-ttu-id="4de62-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="4de62-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="4de62-138">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的设置的读/写访问模式。</span><span class="sxs-lookup"><span data-stu-id="4de62-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="4de62-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="4de62-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="4de62-140">keywords</span><span class="sxs-lookup"><span data-stu-id="4de62-140">keywords</span></span>|<span data-ttu-id="4de62-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="4de62-141">String collection</span></span>|<span data-ttu-id="4de62-142">要在继承自[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)中搜索设置的标记</span><span class="sxs-lookup"><span data-stu-id="4de62-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="4de62-143">infoUrls</span></span>|<span data-ttu-id="4de62-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="4de62-144">String collection</span></span>|<span data-ttu-id="4de62-145">可从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的链接的详细信息列表。</span><span class="sxs-lookup"><span data-stu-id="4de62-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-146">重复</span><span class="sxs-lookup"><span data-stu-id="4de62-146">occurrence</span></span>|[<span data-ttu-id="4de62-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="4de62-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="4de62-148">指示是否需要设置或不继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4de62-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="4de62-149">baseUri</span></span>|<span data-ttu-id="4de62-150">String</span><span class="sxs-lookup"><span data-stu-id="4de62-150">String</span></span>|<span data-ttu-id="4de62-151">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的基本 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="4de62-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="4de62-152">offsetUri</span></span>|<span data-ttu-id="4de62-153">String</span><span class="sxs-lookup"><span data-stu-id="4de62-153">String</span></span>|<span data-ttu-id="4de62-154">从 Base 继承的[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)中偏移 CSP 路径</span><span class="sxs-lookup"><span data-stu-id="4de62-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4de62-155">rootDefinitionId</span></span>|<span data-ttu-id="4de62-156">String</span><span class="sxs-lookup"><span data-stu-id="4de62-156">String</span></span>|<span data-ttu-id="4de62-157">根设置定义（如果设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="4de62-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="4de62-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4de62-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="4de62-159">categoryId</span></span>|<span data-ttu-id="4de62-160">String</span><span class="sxs-lookup"><span data-stu-id="4de62-160">String</span></span>|<span data-ttu-id="4de62-161">指定在指定的配置服务提供程序中配置设置的区域组 (CSP) 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4de62-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="4de62-162">settingUsage</span></span>|[<span data-ttu-id="4de62-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="4de62-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="4de62-164">设置类型，例如，从 [DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的配置和合规性。</span><span class="sxs-lookup"><span data-stu-id="4de62-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="4de62-165">可能的值是：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="4de62-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="4de62-166">id</span><span class="sxs-lookup"><span data-stu-id="4de62-166">id</span></span>|<span data-ttu-id="4de62-167">String</span><span class="sxs-lookup"><span data-stu-id="4de62-167">String</span></span>|<span data-ttu-id="4de62-168">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的标识符</span><span class="sxs-lookup"><span data-stu-id="4de62-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-169">description</span><span class="sxs-lookup"><span data-stu-id="4de62-169">description</span></span>|<span data-ttu-id="4de62-170">String</span><span class="sxs-lookup"><span data-stu-id="4de62-170">String</span></span>|<span data-ttu-id="4de62-171">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的说明</span><span class="sxs-lookup"><span data-stu-id="4de62-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-172">helpText</span><span class="sxs-lookup"><span data-stu-id="4de62-172">helpText</span></span>|<span data-ttu-id="4de62-173">String</span><span class="sxs-lookup"><span data-stu-id="4de62-173">String</span></span>|<span data-ttu-id="4de62-174">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的帮助文本</span><span class="sxs-lookup"><span data-stu-id="4de62-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-175">name</span><span class="sxs-lookup"><span data-stu-id="4de62-175">name</span></span>|<span data-ttu-id="4de62-176">String</span><span class="sxs-lookup"><span data-stu-id="4de62-176">String</span></span>|<span data-ttu-id="4de62-177">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的名称</span><span class="sxs-lookup"><span data-stu-id="4de62-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-178">displayName</span><span class="sxs-lookup"><span data-stu-id="4de62-178">displayName</span></span>|<span data-ttu-id="4de62-179">String</span><span class="sxs-lookup"><span data-stu-id="4de62-179">String</span></span>|<span data-ttu-id="4de62-180">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项的显示名称</span><span class="sxs-lookup"><span data-stu-id="4de62-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-181">version</span><span class="sxs-lookup"><span data-stu-id="4de62-181">version</span></span>|<span data-ttu-id="4de62-182">String</span><span class="sxs-lookup"><span data-stu-id="4de62-182">String</span></span>|<span data-ttu-id="4de62-183">从[DeviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的项目版本</span><span class="sxs-lookup"><span data-stu-id="4de62-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-184">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="4de62-184">valueDefinition</span></span>|[<span data-ttu-id="4de62-185">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="4de62-185">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="4de62-186">此设置从[DeviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)继承的值的定义</span><span class="sxs-lookup"><span data-stu-id="4de62-186">Definition of the value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-187">默认</span><span class="sxs-lookup"><span data-stu-id="4de62-187">defaultValue</span></span>|[<span data-ttu-id="4de62-188">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="4de62-188">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="4de62-189">此设置继承自[deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)的默认设置值</span><span class="sxs-lookup"><span data-stu-id="4de62-189">Default setting value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-190">dependentOn</span><span class="sxs-lookup"><span data-stu-id="4de62-190">dependentOn</span></span>|<span data-ttu-id="4de62-191">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4de62-191">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="4de62-192">父设置列表此设置依赖于从[DeviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)继承的</span><span class="sxs-lookup"><span data-stu-id="4de62-192">list of parent settings this setting is dependent on Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-193">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="4de62-193">dependedOnBy</span></span>|<span data-ttu-id="4de62-194">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4de62-194">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="4de62-195">取决于从[DeviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)继承的此设置的子设置列表</span><span class="sxs-lookup"><span data-stu-id="4de62-195">list of child settings that depend on this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="4de62-196">maximumCount</span><span class="sxs-lookup"><span data-stu-id="4de62-196">maximumCount</span></span>|<span data-ttu-id="4de62-197">Int32</span><span class="sxs-lookup"><span data-stu-id="4de62-197">Int32</span></span>|<span data-ttu-id="4de62-198">集合中简单设置的最大数量。</span><span class="sxs-lookup"><span data-stu-id="4de62-198">Maximum number of simple settings in the collection.</span></span> <span data-ttu-id="4de62-199">有效值为1至100</span><span class="sxs-lookup"><span data-stu-id="4de62-199">Valid values 1 to 100</span></span>|
|<span data-ttu-id="4de62-200">minimumCount</span><span class="sxs-lookup"><span data-stu-id="4de62-200">minimumCount</span></span>|<span data-ttu-id="4de62-201">Int32</span><span class="sxs-lookup"><span data-stu-id="4de62-201">Int32</span></span>|<span data-ttu-id="4de62-202">集合中简单设置的最小数目。</span><span class="sxs-lookup"><span data-stu-id="4de62-202">Minimum number of simple settings in the collection.</span></span> <span data-ttu-id="4de62-203">有效值为1至100</span><span class="sxs-lookup"><span data-stu-id="4de62-203">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="4de62-204">响应</span><span class="sxs-lookup"><span data-stu-id="4de62-204">Response</span></span>
<span data-ttu-id="4de62-205">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4de62-205">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4de62-206">示例</span><span class="sxs-lookup"><span data-stu-id="4de62-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="4de62-207">请求</span><span class="sxs-lookup"><span data-stu-id="4de62-207">Request</span></span>
<span data-ttu-id="4de62-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4de62-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 9183

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionDefinition",
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="4de62-209">响应</span><span class="sxs-lookup"><span data-stu-id="4de62-209">Response</span></span>
<span data-ttu-id="4de62-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4de62-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9232

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionDefinition",
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
  "id": "cb4abda1-bda1-cb4a-a1bd-4acba1bd4acb",
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```




