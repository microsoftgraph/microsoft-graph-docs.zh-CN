---
title: 更新 deviceManagementConfigurationSettingGroupCollectionDefinition
description: 更新 deviceManagementConfigurationSettingGroupCollectionDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d39b342c84dacd6672da163dbcc542fb73771d9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156033"
---
# <a name="update-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="b9f4d-103">更新 deviceManagementConfigurationSettingGroupCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="b9f4d-103">Update deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="b9f4d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9f4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9f4d-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9f4d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9f4d-107">更新 [deviceManagementConfigurationSettingGroupCollectionDefinition 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-107">Update the properties of a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9f4d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9f4d-108">Prerequisites</span></span>
<span data-ttu-id="b9f4d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9f4d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9f4d-111">Permission type</span></span>|<span data-ttu-id="b9f4d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b9f4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9f4d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9f4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9f4d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f4d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9f4d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9f4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9f4d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-116">Not supported.</span></span>|
|<span data-ttu-id="b9f4d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9f4d-117">Application</span></span>|<span data-ttu-id="b9f4d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f4d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9f4d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9f4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="b9f4d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9f4d-120">Request headers</span></span>
|<span data-ttu-id="b9f4d-121">标头</span><span class="sxs-lookup"><span data-stu-id="b9f4d-121">Header</span></span>|<span data-ttu-id="b9f4d-122">值</span><span class="sxs-lookup"><span data-stu-id="b9f4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9f4d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9f4d-123">Authorization</span></span>|<span data-ttu-id="b9f4d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9f4d-125">接受</span><span class="sxs-lookup"><span data-stu-id="b9f4d-125">Accept</span></span>|<span data-ttu-id="b9f4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9f4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9f4d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9f4d-127">Request body</span></span>
<span data-ttu-id="b9f4d-128">在请求正文中，提供 [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

<span data-ttu-id="b9f4d-129">下表显示创建 [deviceManagementConfigurationSettingGroupCollectionDefinition 时所需的属性](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md).</span></span>

|<span data-ttu-id="b9f4d-130">属性</span><span class="sxs-lookup"><span data-stu-id="b9f4d-130">Property</span></span>|<span data-ttu-id="b9f4d-131">类型</span><span class="sxs-lookup"><span data-stu-id="b9f4d-131">Type</span></span>|<span data-ttu-id="b9f4d-132">说明</span><span class="sxs-lookup"><span data-stu-id="b9f4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9f4d-133">适用性</span><span class="sxs-lookup"><span data-stu-id="b9f4d-133">applicability</span></span>|[<span data-ttu-id="b9f4d-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="b9f4d-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="b9f4d-135">有关哪些设备设置适用于继承自 [deviceManagementConfigurationSettingDefinition 的详细信息](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="b9f4d-136">accessTypes</span></span>|[<span data-ttu-id="b9f4d-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="b9f4d-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="b9f4d-138">设置的读/写访问模式 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b9f4d-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="b9f4d-140">keywords</span><span class="sxs-lookup"><span data-stu-id="b9f4d-140">keywords</span></span>|<span data-ttu-id="b9f4d-141">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b9f4d-141">String collection</span></span>|<span data-ttu-id="b9f4d-142">在继承自 [deviceManagementConfigurationSettingDefinition 上搜索设置的令牌](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="b9f4d-143">infoUrls</span></span>|<span data-ttu-id="b9f4d-144">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b9f4d-144">String collection</span></span>|<span data-ttu-id="b9f4d-145">可以在"继承自[deviceManagementConfigurationSettingDefinition"](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)上找到链接列表，了解有关设置详细信息</span><span class="sxs-lookup"><span data-stu-id="b9f4d-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="b9f4d-146">occurrence</span></span>|[<span data-ttu-id="b9f4d-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="b9f4d-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="b9f4d-148">指示设置是否必需。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="b9f4d-149">baseUri</span></span>|<span data-ttu-id="b9f4d-150">String</span><span class="sxs-lookup"><span data-stu-id="b9f4d-150">String</span></span>|<span data-ttu-id="b9f4d-151">基本 CSP 路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="b9f4d-152">offsetUri</span></span>|<span data-ttu-id="b9f4d-153">String</span><span class="sxs-lookup"><span data-stu-id="b9f4d-153">String</span></span>|<span data-ttu-id="b9f4d-154">从 Base 偏移 CSP 路径 继承 [自 deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b9f4d-155">rootDefinitionId</span></span>|<span data-ttu-id="b9f4d-156">String</span><span class="sxs-lookup"><span data-stu-id="b9f4d-156">String</span></span>|<span data-ttu-id="b9f4d-157">根设置定义（如果该设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="b9f4d-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="b9f4d-159">categoryId</span></span>|<span data-ttu-id="b9f4d-160">String</span><span class="sxs-lookup"><span data-stu-id="b9f4d-160">String</span></span>|<span data-ttu-id="b9f4d-161">指定在 CSP) 从[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的指定配置服务提供程序 (配置设置的区域组</span><span class="sxs-lookup"><span data-stu-id="b9f4d-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="b9f4d-162">settingUsage</span></span>|[<span data-ttu-id="b9f4d-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="b9f4d-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="b9f4d-164">设置类型，例如，配置和合规性 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b9f4d-165">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="b9f4d-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="b9f4d-166">uxBehavior</span></span>|[<span data-ttu-id="b9f4d-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="b9f4d-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="b9f4d-168">在 UX 中设置控件类型表示形式 继承 [自 deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b9f4d-169">可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="b9f4d-170">id</span><span class="sxs-lookup"><span data-stu-id="b9f4d-170">id</span></span>|<span data-ttu-id="b9f4d-171">String</span><span class="sxs-lookup"><span data-stu-id="b9f4d-171">String</span></span>|<span data-ttu-id="b9f4d-172">项的标识符 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-172">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-173">说明</span><span class="sxs-lookup"><span data-stu-id="b9f4d-173">description</span></span>|<span data-ttu-id="b9f4d-174">String</span><span class="sxs-lookup"><span data-stu-id="b9f4d-174">String</span></span>|<span data-ttu-id="b9f4d-175">项目说明 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-175">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-176">helpText</span><span class="sxs-lookup"><span data-stu-id="b9f4d-176">helpText</span></span>|<span data-ttu-id="b9f4d-177">String</span><span class="sxs-lookup"><span data-stu-id="b9f4d-177">String</span></span>|<span data-ttu-id="b9f4d-178">项的帮助文本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-178">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-179">名称</span><span class="sxs-lookup"><span data-stu-id="b9f4d-179">name</span></span>|<span data-ttu-id="b9f4d-180">String</span><span class="sxs-lookup"><span data-stu-id="b9f4d-180">String</span></span>|<span data-ttu-id="b9f4d-181">项目名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-181">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-182">displayName</span><span class="sxs-lookup"><span data-stu-id="b9f4d-182">displayName</span></span>|<span data-ttu-id="b9f4d-183">String</span><span class="sxs-lookup"><span data-stu-id="b9f4d-183">String</span></span>|<span data-ttu-id="b9f4d-184">项目的显示名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-184">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-185">version</span><span class="sxs-lookup"><span data-stu-id="b9f4d-185">version</span></span>|<span data-ttu-id="b9f4d-186">String</span><span class="sxs-lookup"><span data-stu-id="b9f4d-186">String</span></span>|<span data-ttu-id="b9f4d-187">项目版本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-187">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-188">childIds</span><span class="sxs-lookup"><span data-stu-id="b9f4d-188">childIds</span></span>|<span data-ttu-id="b9f4d-189">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b9f4d-189">String collection</span></span>|<span data-ttu-id="b9f4d-190">此组设置的依赖子设置 继承自 [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-190">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-191">dependentOn</span><span class="sxs-lookup"><span data-stu-id="b9f4d-191">dependentOn</span></span>|<span data-ttu-id="b9f4d-192">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b9f4d-192">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="b9f4d-193">设置组的依赖关系列表 继承自 [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-193">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-194">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="b9f4d-194">dependedOnBy</span></span>|<span data-ttu-id="b9f4d-195">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b9f4d-195">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="b9f4d-196">依赖于此设置的子设置列表 继承自 [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b9f4d-196">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="b9f4d-197">maximumCount</span><span class="sxs-lookup"><span data-stu-id="b9f4d-197">maximumCount</span></span>|<span data-ttu-id="b9f4d-198">Int32</span><span class="sxs-lookup"><span data-stu-id="b9f4d-198">Int32</span></span>|<span data-ttu-id="b9f4d-199">集合中设置组计数的最大数目。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-199">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="b9f4d-200">有效值为 1 到 100</span><span class="sxs-lookup"><span data-stu-id="b9f4d-200">Valid values 1 to 100</span></span>|
|<span data-ttu-id="b9f4d-201">minimumCount</span><span class="sxs-lookup"><span data-stu-id="b9f4d-201">minimumCount</span></span>|<span data-ttu-id="b9f4d-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b9f4d-202">Int32</span></span>|<span data-ttu-id="b9f4d-203">集合中设置组计数的最小数目。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-203">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="b9f4d-204">有效值为 1 到 100</span><span class="sxs-lookup"><span data-stu-id="b9f4d-204">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="b9f4d-205">响应</span><span class="sxs-lookup"><span data-stu-id="b9f4d-205">Response</span></span>
<span data-ttu-id="b9f4d-206">如果成功，此方法在响应正文中返回响应代码和更新 `200 OK` [的 deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-206">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9f4d-207">示例</span><span class="sxs-lookup"><span data-stu-id="b9f4d-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9f4d-208">请求</span><span class="sxs-lookup"><span data-stu-id="b9f4d-208">Request</span></span>
<span data-ttu-id="b9f4d-209">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1533

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
  "uxBehavior": "dropdown",
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

### <a name="response"></a><span data-ttu-id="b9f4d-210">响应</span><span class="sxs-lookup"><span data-stu-id="b9f4d-210">Response</span></span>
<span data-ttu-id="b9f4d-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9f4d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1582

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
  "uxBehavior": "dropdown",
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




