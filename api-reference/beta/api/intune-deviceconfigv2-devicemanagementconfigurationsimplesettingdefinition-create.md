---
title: 创建 deviceManagementConfigurationSimpleSettingDefinition
description: 创建新的 deviceManagementConfigurationSimpleSettingDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: afba814b56eef8620aa2704c5848671a57b9ff5c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129123"
---
# <a name="create-devicemanagementconfigurationsimplesettingdefinition"></a><span data-ttu-id="e59e5-103">创建 deviceManagementConfigurationSimpleSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="e59e5-103">Create deviceManagementConfigurationSimpleSettingDefinition</span></span>

<span data-ttu-id="e59e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e59e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e59e5-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e59e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e59e5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e59e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e59e5-107">创建新的 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e59e5-107">Create a new [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e59e5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e59e5-108">Prerequisites</span></span>
<span data-ttu-id="e59e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e59e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e59e5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e59e5-111">Permission type</span></span>|<span data-ttu-id="e59e5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e59e5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e59e5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e59e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e59e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e59e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e59e5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e59e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e59e5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e59e5-116">Not supported.</span></span>|
|<span data-ttu-id="e59e5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e59e5-117">Application</span></span>|<span data-ttu-id="e59e5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e59e5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e59e5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e59e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="e59e5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e59e5-120">Request headers</span></span>
|<span data-ttu-id="e59e5-121">标头</span><span class="sxs-lookup"><span data-stu-id="e59e5-121">Header</span></span>|<span data-ttu-id="e59e5-122">值</span><span class="sxs-lookup"><span data-stu-id="e59e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e59e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e59e5-123">Authorization</span></span>|<span data-ttu-id="e59e5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e59e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e59e5-125">接受</span><span class="sxs-lookup"><span data-stu-id="e59e5-125">Accept</span></span>|<span data-ttu-id="e59e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e59e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e59e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e59e5-127">Request body</span></span>
<span data-ttu-id="e59e5-128">在请求正文中，提供 deviceManagementConfigurationSimpleSettingDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e59e5-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSimpleSettingDefinition object.</span></span>

<span data-ttu-id="e59e5-129">下表显示创建 deviceManagementConfigurationSimpleSettingDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e59e5-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSimpleSettingDefinition.</span></span>

|<span data-ttu-id="e59e5-130">属性</span><span class="sxs-lookup"><span data-stu-id="e59e5-130">Property</span></span>|<span data-ttu-id="e59e5-131">类型</span><span class="sxs-lookup"><span data-stu-id="e59e5-131">Type</span></span>|<span data-ttu-id="e59e5-132">说明</span><span class="sxs-lookup"><span data-stu-id="e59e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e59e5-133">适用性</span><span class="sxs-lookup"><span data-stu-id="e59e5-133">applicability</span></span>|[<span data-ttu-id="e59e5-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="e59e5-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="e59e5-135">有关哪些设备设置适用于从[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的详细信息</span><span class="sxs-lookup"><span data-stu-id="e59e5-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="e59e5-136">accessTypes</span></span>|[<span data-ttu-id="e59e5-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="e59e5-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="e59e5-138">读取/写入访问模式的设置 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e59e5-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="e59e5-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="e59e5-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="e59e5-140">keywords</span><span class="sxs-lookup"><span data-stu-id="e59e5-140">keywords</span></span>|<span data-ttu-id="e59e5-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e59e5-141">String collection</span></span>|<span data-ttu-id="e59e5-142">要搜索上设置的令牌 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="e59e5-143">infoUrls</span></span>|<span data-ttu-id="e59e5-144">String collection</span><span class="sxs-lookup"><span data-stu-id="e59e5-144">String collection</span></span>|<span data-ttu-id="e59e5-145">有关设置详细信息的链接列表，可在 Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)找到</span><span class="sxs-lookup"><span data-stu-id="e59e5-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="e59e5-146">occurrence</span></span>|[<span data-ttu-id="e59e5-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="e59e5-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="e59e5-148">指示设置是否必需。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="e59e5-149">baseUri</span></span>|<span data-ttu-id="e59e5-150">String</span><span class="sxs-lookup"><span data-stu-id="e59e5-150">String</span></span>|<span data-ttu-id="e59e5-151">基本云解决方案提供商路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="e59e5-152">offsetUri</span></span>|<span data-ttu-id="e59e5-153">String</span><span class="sxs-lookup"><span data-stu-id="e59e5-153">String</span></span>|<span data-ttu-id="e59e5-154">从基本位置偏移 CSP 路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e59e5-155">rootDefinitionId</span></span>|<span data-ttu-id="e59e5-156">String</span><span class="sxs-lookup"><span data-stu-id="e59e5-156">String</span></span>|<span data-ttu-id="e59e5-157">根设置定义（如果该设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="e59e5-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="e59e5-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="e59e5-159">categoryId</span></span>|<span data-ttu-id="e59e5-160">String</span><span class="sxs-lookup"><span data-stu-id="e59e5-160">String</span></span>|<span data-ttu-id="e59e5-161">指定在 CSP (CSP) 指定的配置服务提供程序中配置设置的区域组。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="e59e5-162">settingUsage</span></span>|[<span data-ttu-id="e59e5-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="e59e5-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="e59e5-164">设置类型，例如，配置和合规性 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e59e5-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="e59e5-165">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="e59e5-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="e59e5-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="e59e5-166">uxBehavior</span></span>|[<span data-ttu-id="e59e5-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="e59e5-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="e59e5-168">设置 UX 中的控件类型表示形式 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e59e5-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="e59e5-169">可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。</span><span class="sxs-lookup"><span data-stu-id="e59e5-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="e59e5-170">visibility</span><span class="sxs-lookup"><span data-stu-id="e59e5-170">visibility</span></span>|[<span data-ttu-id="e59e5-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="e59e5-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="e59e5-172">将可见性范围设置为 UX 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e59e5-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="e59e5-173">可取值为：`none`、`settingsCatalog`、`template`。</span><span class="sxs-lookup"><span data-stu-id="e59e5-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="e59e5-174">id</span><span class="sxs-lookup"><span data-stu-id="e59e5-174">id</span></span>|<span data-ttu-id="e59e5-175">String</span><span class="sxs-lookup"><span data-stu-id="e59e5-175">String</span></span>|<span data-ttu-id="e59e5-176">项目的标识符 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-176">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-177">说明</span><span class="sxs-lookup"><span data-stu-id="e59e5-177">description</span></span>|<span data-ttu-id="e59e5-178">String</span><span class="sxs-lookup"><span data-stu-id="e59e5-178">String</span></span>|<span data-ttu-id="e59e5-179">项目说明 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-179">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-180">helpText</span><span class="sxs-lookup"><span data-stu-id="e59e5-180">helpText</span></span>|<span data-ttu-id="e59e5-181">String</span><span class="sxs-lookup"><span data-stu-id="e59e5-181">String</span></span>|<span data-ttu-id="e59e5-182">项目的帮助文本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-182">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-183">name</span><span class="sxs-lookup"><span data-stu-id="e59e5-183">name</span></span>|<span data-ttu-id="e59e5-184">String</span><span class="sxs-lookup"><span data-stu-id="e59e5-184">String</span></span>|<span data-ttu-id="e59e5-185">项目名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-185">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-186">displayName</span><span class="sxs-lookup"><span data-stu-id="e59e5-186">displayName</span></span>|<span data-ttu-id="e59e5-187">String</span><span class="sxs-lookup"><span data-stu-id="e59e5-187">String</span></span>|<span data-ttu-id="e59e5-188">项目的显示名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-188">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-189">version</span><span class="sxs-lookup"><span data-stu-id="e59e5-189">version</span></span>|<span data-ttu-id="e59e5-190">String</span><span class="sxs-lookup"><span data-stu-id="e59e5-190">String</span></span>|<span data-ttu-id="e59e5-191">项目版本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e59e5-191">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="e59e5-192">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="e59e5-192">valueDefinition</span></span>|[<span data-ttu-id="e59e5-193">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="e59e5-193">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="e59e5-194">此设置的值的定义</span><span class="sxs-lookup"><span data-stu-id="e59e5-194">Definition of the value for this setting</span></span>|
|<span data-ttu-id="e59e5-195">defaultValue</span><span class="sxs-lookup"><span data-stu-id="e59e5-195">defaultValue</span></span>|[<span data-ttu-id="e59e5-196">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="e59e5-196">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="e59e5-197">此设置的默认设置值</span><span class="sxs-lookup"><span data-stu-id="e59e5-197">Default setting value for this setting</span></span>|
|<span data-ttu-id="e59e5-198">dependentOn</span><span class="sxs-lookup"><span data-stu-id="e59e5-198">dependentOn</span></span>|<span data-ttu-id="e59e5-199">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e59e5-199">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="e59e5-200">此设置所依赖的父设置列表</span><span class="sxs-lookup"><span data-stu-id="e59e5-200">list of parent settings this setting is dependent on</span></span>|
|<span data-ttu-id="e59e5-201">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="e59e5-201">dependedOnBy</span></span>|<span data-ttu-id="e59e5-202">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e59e5-202">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="e59e5-203">依赖于此设置的子设置列表</span><span class="sxs-lookup"><span data-stu-id="e59e5-203">list of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="e59e5-204">响应</span><span class="sxs-lookup"><span data-stu-id="e59e5-204">Response</span></span>
<span data-ttu-id="e59e5-205">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e59e5-205">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e59e5-206">示例</span><span class="sxs-lookup"><span data-stu-id="e59e5-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="e59e5-207">请求</span><span class="sxs-lookup"><span data-stu-id="e59e5-207">Request</span></span>
<span data-ttu-id="e59e5-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e59e5-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 9192

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
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
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

### <a name="response"></a><span data-ttu-id="e59e5-209">响应</span><span class="sxs-lookup"><span data-stu-id="e59e5-209">Response</span></span>
<span data-ttu-id="e59e5-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e59e5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9241

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
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
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




