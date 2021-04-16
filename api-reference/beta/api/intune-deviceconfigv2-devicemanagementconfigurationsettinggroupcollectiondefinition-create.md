---
title: 创建 deviceManagementConfigurationSettingGroupCollectionDefinition
description: 创建新的 deviceManagementConfigurationSettingGroupCollectionDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 666954c9428429cba8ffe4963ec53a8d8cfcbaeb
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864415"
---
# <a name="create-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="872c4-103">创建 deviceManagementConfigurationSettingGroupCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="872c4-103">Create deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="872c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="872c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="872c4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="872c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="872c4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="872c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="872c4-107">创建新的 [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="872c4-107">Create a new [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="872c4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="872c4-108">Prerequisites</span></span>
<span data-ttu-id="872c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="872c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="872c4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="872c4-111">Permission type</span></span>|<span data-ttu-id="872c4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="872c4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="872c4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="872c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="872c4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="872c4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="872c4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="872c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="872c4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="872c4-116">Not supported.</span></span>|
|<span data-ttu-id="872c4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="872c4-117">Application</span></span>|<span data-ttu-id="872c4-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="872c4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="872c4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="872c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusableSettings
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="872c4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="872c4-120">Request headers</span></span>
|<span data-ttu-id="872c4-121">标头</span><span class="sxs-lookup"><span data-stu-id="872c4-121">Header</span></span>|<span data-ttu-id="872c4-122">值</span><span class="sxs-lookup"><span data-stu-id="872c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="872c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="872c4-123">Authorization</span></span>|<span data-ttu-id="872c4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="872c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="872c4-125">接受</span><span class="sxs-lookup"><span data-stu-id="872c4-125">Accept</span></span>|<span data-ttu-id="872c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="872c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="872c4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="872c4-127">Request body</span></span>
<span data-ttu-id="872c4-128">在请求正文中，提供 deviceManagementConfigurationSettingGroupCollectionDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="872c4-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupCollectionDefinition object.</span></span>

<span data-ttu-id="872c4-129">下表显示创建 deviceManagementConfigurationSettingGroupCollectionDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="872c4-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupCollectionDefinition.</span></span>

|<span data-ttu-id="872c4-130">属性</span><span class="sxs-lookup"><span data-stu-id="872c4-130">Property</span></span>|<span data-ttu-id="872c4-131">类型</span><span class="sxs-lookup"><span data-stu-id="872c4-131">Type</span></span>|<span data-ttu-id="872c4-132">说明</span><span class="sxs-lookup"><span data-stu-id="872c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="872c4-133">适用性</span><span class="sxs-lookup"><span data-stu-id="872c4-133">applicability</span></span>|[<span data-ttu-id="872c4-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="872c4-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="872c4-135">有关哪些设备设置适用于从[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的详细信息</span><span class="sxs-lookup"><span data-stu-id="872c4-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="872c4-136">accessTypes</span></span>|[<span data-ttu-id="872c4-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="872c4-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="872c4-138">读取/写入访问模式的设置 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="872c4-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="872c4-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="872c4-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="872c4-140">keywords</span><span class="sxs-lookup"><span data-stu-id="872c4-140">keywords</span></span>|<span data-ttu-id="872c4-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="872c4-141">String collection</span></span>|<span data-ttu-id="872c4-142">要搜索上设置的令牌 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="872c4-143">infoUrls</span></span>|<span data-ttu-id="872c4-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="872c4-144">String collection</span></span>|<span data-ttu-id="872c4-145">有关设置详细信息的链接列表，可在 Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)找到</span><span class="sxs-lookup"><span data-stu-id="872c4-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="872c4-146">occurrence</span></span>|[<span data-ttu-id="872c4-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="872c4-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="872c4-148">指示设置是否必需。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="872c4-149">baseUri</span></span>|<span data-ttu-id="872c4-150">String</span><span class="sxs-lookup"><span data-stu-id="872c4-150">String</span></span>|<span data-ttu-id="872c4-151">基本云解决方案提供商路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="872c4-152">offsetUri</span></span>|<span data-ttu-id="872c4-153">String</span><span class="sxs-lookup"><span data-stu-id="872c4-153">String</span></span>|<span data-ttu-id="872c4-154">从基本位置偏移 CSP 路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="872c4-155">rootDefinitionId</span></span>|<span data-ttu-id="872c4-156">String</span><span class="sxs-lookup"><span data-stu-id="872c4-156">String</span></span>|<span data-ttu-id="872c4-157">根设置定义（如果该设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="872c4-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="872c4-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="872c4-159">categoryId</span></span>|<span data-ttu-id="872c4-160">String</span><span class="sxs-lookup"><span data-stu-id="872c4-160">String</span></span>|<span data-ttu-id="872c4-161">指定在 CSP (CSP) 指定的配置服务提供程序中配置设置的区域组。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="872c4-162">settingUsage</span></span>|[<span data-ttu-id="872c4-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="872c4-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="872c4-164">设置类型，例如，配置和合规性 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="872c4-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="872c4-165">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="872c4-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="872c4-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="872c4-166">uxBehavior</span></span>|[<span data-ttu-id="872c4-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="872c4-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="872c4-168">设置 UX 中的控件类型表示形式 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="872c4-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="872c4-169">可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。</span><span class="sxs-lookup"><span data-stu-id="872c4-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="872c4-170">visibility</span><span class="sxs-lookup"><span data-stu-id="872c4-170">visibility</span></span>|[<span data-ttu-id="872c4-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="872c4-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="872c4-172">将可见性范围设置为 UX 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="872c4-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="872c4-173">可取值为：`none`、`settingsCatalog`、`template`。</span><span class="sxs-lookup"><span data-stu-id="872c4-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="872c4-174">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="872c4-174">referredSettingInformationList</span></span>|<span data-ttu-id="872c4-175">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="872c4-175">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="872c4-176">引用的设置信息的列表。</span><span class="sxs-lookup"><span data-stu-id="872c4-176">List of referred setting information.</span></span> <span data-ttu-id="872c4-177">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-177">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-178">id</span><span class="sxs-lookup"><span data-stu-id="872c4-178">id</span></span>|<span data-ttu-id="872c4-179">String</span><span class="sxs-lookup"><span data-stu-id="872c4-179">String</span></span>|<span data-ttu-id="872c4-180">项目的标识符 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-180">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-181">说明</span><span class="sxs-lookup"><span data-stu-id="872c4-181">description</span></span>|<span data-ttu-id="872c4-182">String</span><span class="sxs-lookup"><span data-stu-id="872c4-182">String</span></span>|<span data-ttu-id="872c4-183">项目说明 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-183">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-184">helpText</span><span class="sxs-lookup"><span data-stu-id="872c4-184">helpText</span></span>|<span data-ttu-id="872c4-185">String</span><span class="sxs-lookup"><span data-stu-id="872c4-185">String</span></span>|<span data-ttu-id="872c4-186">项目的帮助文本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-186">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-187">name</span><span class="sxs-lookup"><span data-stu-id="872c4-187">name</span></span>|<span data-ttu-id="872c4-188">String</span><span class="sxs-lookup"><span data-stu-id="872c4-188">String</span></span>|<span data-ttu-id="872c4-189">项目名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-189">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-190">displayName</span><span class="sxs-lookup"><span data-stu-id="872c4-190">displayName</span></span>|<span data-ttu-id="872c4-191">String</span><span class="sxs-lookup"><span data-stu-id="872c4-191">String</span></span>|<span data-ttu-id="872c4-192">项目的显示名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-192">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-193">version</span><span class="sxs-lookup"><span data-stu-id="872c4-193">version</span></span>|<span data-ttu-id="872c4-194">String</span><span class="sxs-lookup"><span data-stu-id="872c4-194">String</span></span>|<span data-ttu-id="872c4-195">项目版本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-195">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="872c4-196">childIds</span><span class="sxs-lookup"><span data-stu-id="872c4-196">childIds</span></span>|<span data-ttu-id="872c4-197">String 集合</span><span class="sxs-lookup"><span data-stu-id="872c4-197">String collection</span></span>|<span data-ttu-id="872c4-198">此组设置的依赖子设置 继承自 [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-198">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="872c4-199">dependentOn</span><span class="sxs-lookup"><span data-stu-id="872c4-199">dependentOn</span></span>|<span data-ttu-id="872c4-200">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="872c4-200">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="872c4-201">设置组的依赖关系列表 继承自 [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-201">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="872c4-202">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="872c4-202">dependedOnBy</span></span>|<span data-ttu-id="872c4-203">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="872c4-203">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="872c4-204">依赖于此设置的子设置列表 继承自 [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="872c4-204">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="872c4-205">maximumCount</span><span class="sxs-lookup"><span data-stu-id="872c4-205">maximumCount</span></span>|<span data-ttu-id="872c4-206">Int32</span><span class="sxs-lookup"><span data-stu-id="872c4-206">Int32</span></span>|<span data-ttu-id="872c4-207">集合中设置组计数的最大数目。</span><span class="sxs-lookup"><span data-stu-id="872c4-207">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="872c4-208">有效值为 1 到 100</span><span class="sxs-lookup"><span data-stu-id="872c4-208">Valid values 1 to 100</span></span>|
|<span data-ttu-id="872c4-209">minimumCount</span><span class="sxs-lookup"><span data-stu-id="872c4-209">minimumCount</span></span>|<span data-ttu-id="872c4-210">Int32</span><span class="sxs-lookup"><span data-stu-id="872c4-210">Int32</span></span>|<span data-ttu-id="872c4-211">集合中设置组计数的最小数目。</span><span class="sxs-lookup"><span data-stu-id="872c4-211">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="872c4-212">有效值为 1 到 100</span><span class="sxs-lookup"><span data-stu-id="872c4-212">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="872c4-213">响应</span><span class="sxs-lookup"><span data-stu-id="872c4-213">Response</span></span>
<span data-ttu-id="872c4-214">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="872c4-214">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="872c4-215">示例</span><span class="sxs-lookup"><span data-stu-id="872c4-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="872c4-216">请求</span><span class="sxs-lookup"><span data-stu-id="872c4-216">Request</span></span>
<span data-ttu-id="872c4-217">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="872c4-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusableSettings
Content-type: application/json
Content-length: 1785

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
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="872c4-218">响应</span><span class="sxs-lookup"><span data-stu-id="872c4-218">Response</span></span>
<span data-ttu-id="872c4-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="872c4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1834

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
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
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




