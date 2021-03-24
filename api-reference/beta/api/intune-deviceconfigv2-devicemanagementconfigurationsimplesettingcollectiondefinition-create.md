---
title: 创建 deviceManagementConfigurationSimpleSettingCollectionDefinition
description: 创建新的 deviceManagementConfigurationSimpleSettingCollectionDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8f1028ea726218f30fe4f4499d60cead5f4472d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129179"
---
# <a name="create-devicemanagementconfigurationsimplesettingcollectiondefinition"></a><span data-ttu-id="9a0c2-103">创建 deviceManagementConfigurationSimpleSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="9a0c2-103">Create deviceManagementConfigurationSimpleSettingCollectionDefinition</span></span>

<span data-ttu-id="9a0c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a0c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a0c2-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a0c2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a0c2-107">创建新的 [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-107">Create a new [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a0c2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9a0c2-108">Prerequisites</span></span>
<span data-ttu-id="9a0c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a0c2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a0c2-111">Permission type</span></span>|<span data-ttu-id="9a0c2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a0c2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a0c2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a0c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a0c2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a0c2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a0c2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a0c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a0c2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-116">Not supported.</span></span>|
|<span data-ttu-id="9a0c2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a0c2-117">Application</span></span>|<span data-ttu-id="9a0c2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a0c2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a0c2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a0c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="9a0c2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a0c2-120">Request headers</span></span>
|<span data-ttu-id="9a0c2-121">标头</span><span class="sxs-lookup"><span data-stu-id="9a0c2-121">Header</span></span>|<span data-ttu-id="9a0c2-122">值</span><span class="sxs-lookup"><span data-stu-id="9a0c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a0c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a0c2-123">Authorization</span></span>|<span data-ttu-id="9a0c2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a0c2-125">接受</span><span class="sxs-lookup"><span data-stu-id="9a0c2-125">Accept</span></span>|<span data-ttu-id="9a0c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a0c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a0c2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a0c2-127">Request body</span></span>
<span data-ttu-id="9a0c2-128">在请求正文中，提供 deviceManagementConfigurationSimpleSettingCollectionDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSimpleSettingCollectionDefinition object.</span></span>

<span data-ttu-id="9a0c2-129">下表显示创建 deviceManagementConfigurationSimpleSettingCollectionDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSimpleSettingCollectionDefinition.</span></span>

|<span data-ttu-id="9a0c2-130">属性</span><span class="sxs-lookup"><span data-stu-id="9a0c2-130">Property</span></span>|<span data-ttu-id="9a0c2-131">类型</span><span class="sxs-lookup"><span data-stu-id="9a0c2-131">Type</span></span>|<span data-ttu-id="9a0c2-132">说明</span><span class="sxs-lookup"><span data-stu-id="9a0c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a0c2-133">适用性</span><span class="sxs-lookup"><span data-stu-id="9a0c2-133">applicability</span></span>|[<span data-ttu-id="9a0c2-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="9a0c2-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="9a0c2-135">有关哪些设备设置适用于从[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的详细信息</span><span class="sxs-lookup"><span data-stu-id="9a0c2-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="9a0c2-136">accessTypes</span></span>|[<span data-ttu-id="9a0c2-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="9a0c2-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="9a0c2-138">读取/写入访问模式的设置 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="9a0c2-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="9a0c2-140">keywords</span><span class="sxs-lookup"><span data-stu-id="9a0c2-140">keywords</span></span>|<span data-ttu-id="9a0c2-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9a0c2-141">String collection</span></span>|<span data-ttu-id="9a0c2-142">要搜索上设置的令牌 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="9a0c2-143">infoUrls</span></span>|<span data-ttu-id="9a0c2-144">String collection</span><span class="sxs-lookup"><span data-stu-id="9a0c2-144">String collection</span></span>|<span data-ttu-id="9a0c2-145">有关设置详细信息的链接列表，可在 Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)找到</span><span class="sxs-lookup"><span data-stu-id="9a0c2-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="9a0c2-146">occurrence</span></span>|[<span data-ttu-id="9a0c2-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="9a0c2-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="9a0c2-148">指示设置是否必需。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="9a0c2-149">baseUri</span></span>|<span data-ttu-id="9a0c2-150">String</span><span class="sxs-lookup"><span data-stu-id="9a0c2-150">String</span></span>|<span data-ttu-id="9a0c2-151">基本云解决方案提供商路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="9a0c2-152">offsetUri</span></span>|<span data-ttu-id="9a0c2-153">String</span><span class="sxs-lookup"><span data-stu-id="9a0c2-153">String</span></span>|<span data-ttu-id="9a0c2-154">从基本位置偏移 CSP 路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9a0c2-155">rootDefinitionId</span></span>|<span data-ttu-id="9a0c2-156">String</span><span class="sxs-lookup"><span data-stu-id="9a0c2-156">String</span></span>|<span data-ttu-id="9a0c2-157">根设置定义（如果该设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="9a0c2-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="9a0c2-159">categoryId</span></span>|<span data-ttu-id="9a0c2-160">String</span><span class="sxs-lookup"><span data-stu-id="9a0c2-160">String</span></span>|<span data-ttu-id="9a0c2-161">指定在 CSP (CSP) 指定的配置服务提供程序中配置设置的区域组。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="9a0c2-162">settingUsage</span></span>|[<span data-ttu-id="9a0c2-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="9a0c2-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="9a0c2-164">设置类型，例如，配置和合规性 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="9a0c2-165">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="9a0c2-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="9a0c2-166">uxBehavior</span></span>|[<span data-ttu-id="9a0c2-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="9a0c2-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="9a0c2-168">设置 UX 中的控件类型表示形式 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="9a0c2-169">可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="9a0c2-170">visibility</span><span class="sxs-lookup"><span data-stu-id="9a0c2-170">visibility</span></span>|[<span data-ttu-id="9a0c2-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="9a0c2-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="9a0c2-172">将可见性范围设置为 UX 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="9a0c2-173">可取值为：`none`、`settingsCatalog`、`template`。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="9a0c2-174">id</span><span class="sxs-lookup"><span data-stu-id="9a0c2-174">id</span></span>|<span data-ttu-id="9a0c2-175">String</span><span class="sxs-lookup"><span data-stu-id="9a0c2-175">String</span></span>|<span data-ttu-id="9a0c2-176">项目的标识符 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-176">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-177">说明</span><span class="sxs-lookup"><span data-stu-id="9a0c2-177">description</span></span>|<span data-ttu-id="9a0c2-178">String</span><span class="sxs-lookup"><span data-stu-id="9a0c2-178">String</span></span>|<span data-ttu-id="9a0c2-179">项目说明 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-179">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-180">helpText</span><span class="sxs-lookup"><span data-stu-id="9a0c2-180">helpText</span></span>|<span data-ttu-id="9a0c2-181">String</span><span class="sxs-lookup"><span data-stu-id="9a0c2-181">String</span></span>|<span data-ttu-id="9a0c2-182">项目的帮助文本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-182">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-183">name</span><span class="sxs-lookup"><span data-stu-id="9a0c2-183">name</span></span>|<span data-ttu-id="9a0c2-184">String</span><span class="sxs-lookup"><span data-stu-id="9a0c2-184">String</span></span>|<span data-ttu-id="9a0c2-185">项目名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-185">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-186">displayName</span><span class="sxs-lookup"><span data-stu-id="9a0c2-186">displayName</span></span>|<span data-ttu-id="9a0c2-187">String</span><span class="sxs-lookup"><span data-stu-id="9a0c2-187">String</span></span>|<span data-ttu-id="9a0c2-188">项目的显示名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-188">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-189">version</span><span class="sxs-lookup"><span data-stu-id="9a0c2-189">version</span></span>|<span data-ttu-id="9a0c2-190">String</span><span class="sxs-lookup"><span data-stu-id="9a0c2-190">String</span></span>|<span data-ttu-id="9a0c2-191">项目版本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-191">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-192">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="9a0c2-192">valueDefinition</span></span>|[<span data-ttu-id="9a0c2-193">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="9a0c2-193">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="9a0c2-194">此设置的值定义 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-194">Definition of the value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-195">defaultValue</span><span class="sxs-lookup"><span data-stu-id="9a0c2-195">defaultValue</span></span>|[<span data-ttu-id="9a0c2-196">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="9a0c2-196">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="9a0c2-197">此设置的默认设置值 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-197">Default setting value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-198">dependentOn</span><span class="sxs-lookup"><span data-stu-id="9a0c2-198">dependentOn</span></span>|<span data-ttu-id="9a0c2-199">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a0c2-199">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="9a0c2-200">此设置依赖于父设置列表 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-200">list of parent settings this setting is dependent on Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-201">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="9a0c2-201">dependedOnBy</span></span>|<span data-ttu-id="9a0c2-202">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a0c2-202">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="9a0c2-203">依赖于此设置的子设置列表 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9a0c2-203">list of child settings that depend on this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="9a0c2-204">maximumCount</span><span class="sxs-lookup"><span data-stu-id="9a0c2-204">maximumCount</span></span>|<span data-ttu-id="9a0c2-205">Int32</span><span class="sxs-lookup"><span data-stu-id="9a0c2-205">Int32</span></span>|<span data-ttu-id="9a0c2-206">集合中简单设置的最大数目。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-206">Maximum number of simple settings in the collection.</span></span> <span data-ttu-id="9a0c2-207">有效值为 1 到 100</span><span class="sxs-lookup"><span data-stu-id="9a0c2-207">Valid values 1 to 100</span></span>|
|<span data-ttu-id="9a0c2-208">minimumCount</span><span class="sxs-lookup"><span data-stu-id="9a0c2-208">minimumCount</span></span>|<span data-ttu-id="9a0c2-209">Int32</span><span class="sxs-lookup"><span data-stu-id="9a0c2-209">Int32</span></span>|<span data-ttu-id="9a0c2-210">集合中的最小简单设置数。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-210">Minimum number of simple settings in the collection.</span></span> <span data-ttu-id="9a0c2-211">有效值为 1 到 100</span><span class="sxs-lookup"><span data-stu-id="9a0c2-211">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="9a0c2-212">响应</span><span class="sxs-lookup"><span data-stu-id="9a0c2-212">Response</span></span>
<span data-ttu-id="9a0c2-213">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-213">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a0c2-214">示例</span><span class="sxs-lookup"><span data-stu-id="9a0c2-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a0c2-215">请求</span><span class="sxs-lookup"><span data-stu-id="9a0c2-215">Request</span></span>
<span data-ttu-id="9a0c2-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 9248

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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="9a0c2-217">响应</span><span class="sxs-lookup"><span data-stu-id="9a0c2-217">Response</span></span>
<span data-ttu-id="9a0c2-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a0c2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9297

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
  "visibility": "settingsCatalog",
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




