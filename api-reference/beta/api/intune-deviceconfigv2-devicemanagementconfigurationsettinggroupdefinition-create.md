---
title: 创建 deviceManagementConfigurationSettingGroupDefinition
description: 创建新的 deviceManagementConfigurationSettingGroupDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3a0ea4d784fb91ee237b5bb2de7864dfb1dc5cd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129243"
---
# <a name="create-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="5d7af-103">创建 deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="5d7af-103">Create deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="5d7af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d7af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d7af-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5d7af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d7af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5d7af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d7af-107">创建新的 [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d7af-107">Create a new [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d7af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5d7af-108">Prerequisites</span></span>
<span data-ttu-id="5d7af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d7af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d7af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d7af-111">Permission type</span></span>|<span data-ttu-id="5d7af-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d7af-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d7af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d7af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d7af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d7af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5d7af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d7af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d7af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d7af-116">Not supported.</span></span>|
|<span data-ttu-id="5d7af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d7af-117">Application</span></span>|<span data-ttu-id="5d7af-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d7af-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d7af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d7af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="5d7af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d7af-120">Request headers</span></span>
|<span data-ttu-id="5d7af-121">标头</span><span class="sxs-lookup"><span data-stu-id="5d7af-121">Header</span></span>|<span data-ttu-id="5d7af-122">值</span><span class="sxs-lookup"><span data-stu-id="5d7af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d7af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d7af-123">Authorization</span></span>|<span data-ttu-id="5d7af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5d7af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d7af-125">接受</span><span class="sxs-lookup"><span data-stu-id="5d7af-125">Accept</span></span>|<span data-ttu-id="5d7af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d7af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d7af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d7af-127">Request body</span></span>
<span data-ttu-id="5d7af-128">在请求正文中，提供 deviceManagementConfigurationSettingGroupDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d7af-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupDefinition object.</span></span>

<span data-ttu-id="5d7af-129">下表显示创建 deviceManagementConfigurationSettingGroupDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5d7af-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupDefinition.</span></span>

|<span data-ttu-id="5d7af-130">属性</span><span class="sxs-lookup"><span data-stu-id="5d7af-130">Property</span></span>|<span data-ttu-id="5d7af-131">类型</span><span class="sxs-lookup"><span data-stu-id="5d7af-131">Type</span></span>|<span data-ttu-id="5d7af-132">说明</span><span class="sxs-lookup"><span data-stu-id="5d7af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d7af-133">适用性</span><span class="sxs-lookup"><span data-stu-id="5d7af-133">applicability</span></span>|[<span data-ttu-id="5d7af-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="5d7af-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="5d7af-135">有关哪些设备设置适用于从[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的详细信息</span><span class="sxs-lookup"><span data-stu-id="5d7af-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="5d7af-136">accessTypes</span></span>|[<span data-ttu-id="5d7af-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="5d7af-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="5d7af-138">读取/写入访问模式的设置 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="5d7af-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="5d7af-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="5d7af-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="5d7af-140">keywords</span><span class="sxs-lookup"><span data-stu-id="5d7af-140">keywords</span></span>|<span data-ttu-id="5d7af-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5d7af-141">String collection</span></span>|<span data-ttu-id="5d7af-142">要搜索上设置的令牌 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="5d7af-143">infoUrls</span></span>|<span data-ttu-id="5d7af-144">String collection</span><span class="sxs-lookup"><span data-stu-id="5d7af-144">String collection</span></span>|<span data-ttu-id="5d7af-145">有关设置详细信息的链接列表，可在 Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)找到</span><span class="sxs-lookup"><span data-stu-id="5d7af-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="5d7af-146">occurrence</span></span>|[<span data-ttu-id="5d7af-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="5d7af-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="5d7af-148">指示设置是否必需。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="5d7af-149">baseUri</span></span>|<span data-ttu-id="5d7af-150">String</span><span class="sxs-lookup"><span data-stu-id="5d7af-150">String</span></span>|<span data-ttu-id="5d7af-151">基本云解决方案提供商路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="5d7af-152">offsetUri</span></span>|<span data-ttu-id="5d7af-153">String</span><span class="sxs-lookup"><span data-stu-id="5d7af-153">String</span></span>|<span data-ttu-id="5d7af-154">从基本位置偏移 CSP 路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5d7af-155">rootDefinitionId</span></span>|<span data-ttu-id="5d7af-156">String</span><span class="sxs-lookup"><span data-stu-id="5d7af-156">String</span></span>|<span data-ttu-id="5d7af-157">根设置定义（如果该设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="5d7af-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="5d7af-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="5d7af-159">categoryId</span></span>|<span data-ttu-id="5d7af-160">String</span><span class="sxs-lookup"><span data-stu-id="5d7af-160">String</span></span>|<span data-ttu-id="5d7af-161">指定在 CSP (CSP) 指定的配置服务提供程序中配置设置的区域组。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="5d7af-162">settingUsage</span></span>|[<span data-ttu-id="5d7af-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="5d7af-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="5d7af-164">设置类型，例如，配置和合规性 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="5d7af-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="5d7af-165">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="5d7af-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="5d7af-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="5d7af-166">uxBehavior</span></span>|[<span data-ttu-id="5d7af-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="5d7af-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="5d7af-168">设置 UX 中的控件类型表示形式 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="5d7af-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="5d7af-169">可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。</span><span class="sxs-lookup"><span data-stu-id="5d7af-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="5d7af-170">visibility</span><span class="sxs-lookup"><span data-stu-id="5d7af-170">visibility</span></span>|[<span data-ttu-id="5d7af-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="5d7af-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="5d7af-172">将可见性范围设置为 UX 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="5d7af-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="5d7af-173">可取值为：`none`、`settingsCatalog`、`template`。</span><span class="sxs-lookup"><span data-stu-id="5d7af-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="5d7af-174">id</span><span class="sxs-lookup"><span data-stu-id="5d7af-174">id</span></span>|<span data-ttu-id="5d7af-175">String</span><span class="sxs-lookup"><span data-stu-id="5d7af-175">String</span></span>|<span data-ttu-id="5d7af-176">项目的标识符 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-176">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-177">说明</span><span class="sxs-lookup"><span data-stu-id="5d7af-177">description</span></span>|<span data-ttu-id="5d7af-178">String</span><span class="sxs-lookup"><span data-stu-id="5d7af-178">String</span></span>|<span data-ttu-id="5d7af-179">项目说明 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-179">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-180">helpText</span><span class="sxs-lookup"><span data-stu-id="5d7af-180">helpText</span></span>|<span data-ttu-id="5d7af-181">String</span><span class="sxs-lookup"><span data-stu-id="5d7af-181">String</span></span>|<span data-ttu-id="5d7af-182">项目的帮助文本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-182">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-183">name</span><span class="sxs-lookup"><span data-stu-id="5d7af-183">name</span></span>|<span data-ttu-id="5d7af-184">String</span><span class="sxs-lookup"><span data-stu-id="5d7af-184">String</span></span>|<span data-ttu-id="5d7af-185">项目名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-185">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-186">displayName</span><span class="sxs-lookup"><span data-stu-id="5d7af-186">displayName</span></span>|<span data-ttu-id="5d7af-187">String</span><span class="sxs-lookup"><span data-stu-id="5d7af-187">String</span></span>|<span data-ttu-id="5d7af-188">项目的显示名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-188">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-189">version</span><span class="sxs-lookup"><span data-stu-id="5d7af-189">version</span></span>|<span data-ttu-id="5d7af-190">String</span><span class="sxs-lookup"><span data-stu-id="5d7af-190">String</span></span>|<span data-ttu-id="5d7af-191">项目版本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5d7af-191">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5d7af-192">childIds</span><span class="sxs-lookup"><span data-stu-id="5d7af-192">childIds</span></span>|<span data-ttu-id="5d7af-193">String collection</span><span class="sxs-lookup"><span data-stu-id="5d7af-193">String collection</span></span>|<span data-ttu-id="5d7af-194">此组设置的依赖子设置</span><span class="sxs-lookup"><span data-stu-id="5d7af-194">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="5d7af-195">dependentOn</span><span class="sxs-lookup"><span data-stu-id="5d7af-195">dependentOn</span></span>|<span data-ttu-id="5d7af-196">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5d7af-196">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="5d7af-197">设置组的依赖关系列表</span><span class="sxs-lookup"><span data-stu-id="5d7af-197">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="5d7af-198">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="5d7af-198">dependedOnBy</span></span>|<span data-ttu-id="5d7af-199">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5d7af-199">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="5d7af-200">依赖于此设置的子设置列表</span><span class="sxs-lookup"><span data-stu-id="5d7af-200">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="5d7af-201">响应</span><span class="sxs-lookup"><span data-stu-id="5d7af-201">Response</span></span>
<span data-ttu-id="5d7af-202">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d7af-202">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d7af-203">示例</span><span class="sxs-lookup"><span data-stu-id="5d7af-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d7af-204">请求</span><span class="sxs-lookup"><span data-stu-id="5d7af-204">Request</span></span>
<span data-ttu-id="5d7af-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5d7af-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 1513

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
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
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

### <a name="response"></a><span data-ttu-id="5d7af-206">响应</span><span class="sxs-lookup"><span data-stu-id="5d7af-206">Response</span></span>
<span data-ttu-id="5d7af-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5d7af-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1562

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
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
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




