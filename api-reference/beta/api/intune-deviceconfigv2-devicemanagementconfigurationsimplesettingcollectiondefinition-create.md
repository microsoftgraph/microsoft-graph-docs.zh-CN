---
title: 创建 deviceManagementConfigurationSimpleSettingCollectionDefinition
description: 创建新的 deviceManagementConfigurationSimpleSettingCollectionDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 660b641c7dbbbf89fe653c8f7ec4d0f8ad591279
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158889"
---
# <a name="create-devicemanagementconfigurationsimplesettingcollectiondefinition"></a><span data-ttu-id="92ad7-103">创建 deviceManagementConfigurationSimpleSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="92ad7-103">Create deviceManagementConfigurationSimpleSettingCollectionDefinition</span></span>

<span data-ttu-id="92ad7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92ad7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92ad7-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92ad7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92ad7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92ad7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92ad7-107">创建新的 [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92ad7-107">Create a new [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92ad7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="92ad7-108">Prerequisites</span></span>
<span data-ttu-id="92ad7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92ad7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ad7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="92ad7-111">Permission type</span></span>|<span data-ttu-id="92ad7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="92ad7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92ad7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92ad7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92ad7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92ad7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92ad7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92ad7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92ad7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="92ad7-116">Not supported.</span></span>|
|<span data-ttu-id="92ad7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="92ad7-117">Application</span></span>|<span data-ttu-id="92ad7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92ad7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92ad7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92ad7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="92ad7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="92ad7-120">Request headers</span></span>
|<span data-ttu-id="92ad7-121">标头</span><span class="sxs-lookup"><span data-stu-id="92ad7-121">Header</span></span>|<span data-ttu-id="92ad7-122">值</span><span class="sxs-lookup"><span data-stu-id="92ad7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92ad7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="92ad7-123">Authorization</span></span>|<span data-ttu-id="92ad7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="92ad7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92ad7-125">接受</span><span class="sxs-lookup"><span data-stu-id="92ad7-125">Accept</span></span>|<span data-ttu-id="92ad7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92ad7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92ad7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="92ad7-127">Request body</span></span>
<span data-ttu-id="92ad7-128">在请求正文中，提供 deviceManagementConfigurationSimpleSettingCollectionDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92ad7-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSimpleSettingCollectionDefinition object.</span></span>

<span data-ttu-id="92ad7-129">下表显示创建 deviceManagementConfigurationSimpleSettingCollectionDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="92ad7-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSimpleSettingCollectionDefinition.</span></span>

|<span data-ttu-id="92ad7-130">属性</span><span class="sxs-lookup"><span data-stu-id="92ad7-130">Property</span></span>|<span data-ttu-id="92ad7-131">类型</span><span class="sxs-lookup"><span data-stu-id="92ad7-131">Type</span></span>|<span data-ttu-id="92ad7-132">说明</span><span class="sxs-lookup"><span data-stu-id="92ad7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92ad7-133">适用性</span><span class="sxs-lookup"><span data-stu-id="92ad7-133">applicability</span></span>|[<span data-ttu-id="92ad7-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="92ad7-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="92ad7-135">有关哪些设备设置适用于继承自 [deviceManagementConfigurationSettingDefinition 的详细信息](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="92ad7-136">accessTypes</span></span>|[<span data-ttu-id="92ad7-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="92ad7-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="92ad7-138">设置的读/写访问模式 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="92ad7-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="92ad7-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="92ad7-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="92ad7-140">keywords</span><span class="sxs-lookup"><span data-stu-id="92ad7-140">keywords</span></span>|<span data-ttu-id="92ad7-141">字符串集合</span><span class="sxs-lookup"><span data-stu-id="92ad7-141">String collection</span></span>|<span data-ttu-id="92ad7-142">在继承自 [deviceManagementConfigurationSettingDefinition 上搜索设置的令牌](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="92ad7-143">infoUrls</span></span>|<span data-ttu-id="92ad7-144">字符串集合</span><span class="sxs-lookup"><span data-stu-id="92ad7-144">String collection</span></span>|<span data-ttu-id="92ad7-145">可以在"继承自[deviceManagementConfigurationSettingDefinition"](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)上找到链接列表，了解有关设置详细信息</span><span class="sxs-lookup"><span data-stu-id="92ad7-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="92ad7-146">occurrence</span></span>|[<span data-ttu-id="92ad7-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="92ad7-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="92ad7-148">指示设置是否必需。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="92ad7-149">baseUri</span></span>|<span data-ttu-id="92ad7-150">String</span><span class="sxs-lookup"><span data-stu-id="92ad7-150">String</span></span>|<span data-ttu-id="92ad7-151">基本 CSP 路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="92ad7-152">offsetUri</span></span>|<span data-ttu-id="92ad7-153">String</span><span class="sxs-lookup"><span data-stu-id="92ad7-153">String</span></span>|<span data-ttu-id="92ad7-154">从 Base 偏移 CSP 路径 继承 [自 deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="92ad7-155">rootDefinitionId</span></span>|<span data-ttu-id="92ad7-156">String</span><span class="sxs-lookup"><span data-stu-id="92ad7-156">String</span></span>|<span data-ttu-id="92ad7-157">根设置定义（如果该设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="92ad7-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="92ad7-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="92ad7-159">categoryId</span></span>|<span data-ttu-id="92ad7-160">String</span><span class="sxs-lookup"><span data-stu-id="92ad7-160">String</span></span>|<span data-ttu-id="92ad7-161">指定在 CSP) 从[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的指定配置服务提供程序 (配置设置的区域组</span><span class="sxs-lookup"><span data-stu-id="92ad7-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="92ad7-162">settingUsage</span></span>|[<span data-ttu-id="92ad7-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="92ad7-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="92ad7-164">设置类型，例如，配置和合规性 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="92ad7-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="92ad7-165">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="92ad7-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="92ad7-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="92ad7-166">uxBehavior</span></span>|[<span data-ttu-id="92ad7-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="92ad7-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="92ad7-168">在 UX 中设置控件类型表示形式 继承 [自 deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="92ad7-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="92ad7-169">可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。</span><span class="sxs-lookup"><span data-stu-id="92ad7-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="92ad7-170">id</span><span class="sxs-lookup"><span data-stu-id="92ad7-170">id</span></span>|<span data-ttu-id="92ad7-171">String</span><span class="sxs-lookup"><span data-stu-id="92ad7-171">String</span></span>|<span data-ttu-id="92ad7-172">项的标识符 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-172">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-173">说明</span><span class="sxs-lookup"><span data-stu-id="92ad7-173">description</span></span>|<span data-ttu-id="92ad7-174">String</span><span class="sxs-lookup"><span data-stu-id="92ad7-174">String</span></span>|<span data-ttu-id="92ad7-175">项目说明 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-175">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-176">helpText</span><span class="sxs-lookup"><span data-stu-id="92ad7-176">helpText</span></span>|<span data-ttu-id="92ad7-177">String</span><span class="sxs-lookup"><span data-stu-id="92ad7-177">String</span></span>|<span data-ttu-id="92ad7-178">项的帮助文本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-178">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-179">名称</span><span class="sxs-lookup"><span data-stu-id="92ad7-179">name</span></span>|<span data-ttu-id="92ad7-180">String</span><span class="sxs-lookup"><span data-stu-id="92ad7-180">String</span></span>|<span data-ttu-id="92ad7-181">项目名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-181">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-182">displayName</span><span class="sxs-lookup"><span data-stu-id="92ad7-182">displayName</span></span>|<span data-ttu-id="92ad7-183">String</span><span class="sxs-lookup"><span data-stu-id="92ad7-183">String</span></span>|<span data-ttu-id="92ad7-184">项目的显示名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-184">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-185">version</span><span class="sxs-lookup"><span data-stu-id="92ad7-185">version</span></span>|<span data-ttu-id="92ad7-186">String</span><span class="sxs-lookup"><span data-stu-id="92ad7-186">String</span></span>|<span data-ttu-id="92ad7-187">项目版本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-187">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-188">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="92ad7-188">valueDefinition</span></span>|[<span data-ttu-id="92ad7-189">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="92ad7-189">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="92ad7-190">此设置的值的定义 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-190">Definition of the value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-191">defaultValue</span><span class="sxs-lookup"><span data-stu-id="92ad7-191">defaultValue</span></span>|[<span data-ttu-id="92ad7-192">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="92ad7-192">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="92ad7-193">此设置的默认设置值 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-193">Default setting value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-194">dependentOn</span><span class="sxs-lookup"><span data-stu-id="92ad7-194">dependentOn</span></span>|<span data-ttu-id="92ad7-195">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92ad7-195">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="92ad7-196">此设置所依赖的父设置列表 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-196">list of parent settings this setting is dependent on Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-197">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="92ad7-197">dependedOnBy</span></span>|<span data-ttu-id="92ad7-198">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92ad7-198">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="92ad7-199">依赖于此设置的子设置列表 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ad7-199">list of child settings that depend on this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="92ad7-200">maximumCount</span><span class="sxs-lookup"><span data-stu-id="92ad7-200">maximumCount</span></span>|<span data-ttu-id="92ad7-201">Int32</span><span class="sxs-lookup"><span data-stu-id="92ad7-201">Int32</span></span>|<span data-ttu-id="92ad7-202">集合中简单设置的最大数目。</span><span class="sxs-lookup"><span data-stu-id="92ad7-202">Maximum number of simple settings in the collection.</span></span> <span data-ttu-id="92ad7-203">有效值为 1 到 100</span><span class="sxs-lookup"><span data-stu-id="92ad7-203">Valid values 1 to 100</span></span>|
|<span data-ttu-id="92ad7-204">minimumCount</span><span class="sxs-lookup"><span data-stu-id="92ad7-204">minimumCount</span></span>|<span data-ttu-id="92ad7-205">Int32</span><span class="sxs-lookup"><span data-stu-id="92ad7-205">Int32</span></span>|<span data-ttu-id="92ad7-206">集合中简单设置的最小数量。</span><span class="sxs-lookup"><span data-stu-id="92ad7-206">Minimum number of simple settings in the collection.</span></span> <span data-ttu-id="92ad7-207">有效值为 1 到 100</span><span class="sxs-lookup"><span data-stu-id="92ad7-207">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="92ad7-208">响应</span><span class="sxs-lookup"><span data-stu-id="92ad7-208">Response</span></span>
<span data-ttu-id="92ad7-209">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92ad7-209">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92ad7-210">示例</span><span class="sxs-lookup"><span data-stu-id="92ad7-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="92ad7-211">请求</span><span class="sxs-lookup"><span data-stu-id="92ad7-211">Request</span></span>
<span data-ttu-id="92ad7-212">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92ad7-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 9212

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
  "uxBehavior": "dropdown",
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

### <a name="response"></a><span data-ttu-id="92ad7-213">响应</span><span class="sxs-lookup"><span data-stu-id="92ad7-213">Response</span></span>
<span data-ttu-id="92ad7-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92ad7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9261

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
  "uxBehavior": "dropdown",
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




