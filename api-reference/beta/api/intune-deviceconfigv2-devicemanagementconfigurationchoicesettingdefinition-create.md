---
title: 创建 deviceManagementConfigurationChoiceSettingDefinition
description: 创建新的 deviceManagementConfigurationChoiceSettingDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a8f19a34a1464e76b7cde03c6cbe2975b1360dc
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158637"
---
# <a name="create-devicemanagementconfigurationchoicesettingdefinition"></a><span data-ttu-id="7dce3-103">创建 deviceManagementConfigurationChoiceSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="7dce3-103">Create deviceManagementConfigurationChoiceSettingDefinition</span></span>

<span data-ttu-id="7dce3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dce3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7dce3-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7dce3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dce3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7dce3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dce3-107">创建新的 [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7dce3-107">Create a new [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dce3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7dce3-108">Prerequisites</span></span>
<span data-ttu-id="7dce3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7dce3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dce3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7dce3-111">Permission type</span></span>|<span data-ttu-id="7dce3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7dce3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dce3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7dce3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7dce3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dce3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7dce3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7dce3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dce3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dce3-116">Not supported.</span></span>|
|<span data-ttu-id="7dce3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7dce3-117">Application</span></span>|<span data-ttu-id="7dce3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dce3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dce3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7dce3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="7dce3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7dce3-120">Request headers</span></span>
|<span data-ttu-id="7dce3-121">标头</span><span class="sxs-lookup"><span data-stu-id="7dce3-121">Header</span></span>|<span data-ttu-id="7dce3-122">值</span><span class="sxs-lookup"><span data-stu-id="7dce3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dce3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dce3-123">Authorization</span></span>|<span data-ttu-id="7dce3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7dce3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dce3-125">接受</span><span class="sxs-lookup"><span data-stu-id="7dce3-125">Accept</span></span>|<span data-ttu-id="7dce3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7dce3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dce3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7dce3-127">Request body</span></span>
<span data-ttu-id="7dce3-128">在请求正文中，提供 deviceManagementConfigurationChoiceSettingDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7dce3-128">In the request body, supply a JSON representation for the deviceManagementConfigurationChoiceSettingDefinition object.</span></span>

<span data-ttu-id="7dce3-129">下表显示创建 deviceManagementConfigurationChoiceSettingDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7dce3-129">The following table shows the properties that are required when you create the deviceManagementConfigurationChoiceSettingDefinition.</span></span>

|<span data-ttu-id="7dce3-130">属性</span><span class="sxs-lookup"><span data-stu-id="7dce3-130">Property</span></span>|<span data-ttu-id="7dce3-131">类型</span><span class="sxs-lookup"><span data-stu-id="7dce3-131">Type</span></span>|<span data-ttu-id="7dce3-132">说明</span><span class="sxs-lookup"><span data-stu-id="7dce3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dce3-133">适用性</span><span class="sxs-lookup"><span data-stu-id="7dce3-133">applicability</span></span>|[<span data-ttu-id="7dce3-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="7dce3-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="7dce3-135">有关哪些设备设置适用于继承自 [deviceManagementConfigurationSettingDefinition 的详细信息](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="7dce3-136">accessTypes</span></span>|[<span data-ttu-id="7dce3-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="7dce3-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="7dce3-138">设置的读/写访问模式 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="7dce3-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="7dce3-139">可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。</span><span class="sxs-lookup"><span data-stu-id="7dce3-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="7dce3-140">keywords</span><span class="sxs-lookup"><span data-stu-id="7dce3-140">keywords</span></span>|<span data-ttu-id="7dce3-141">字符串集合</span><span class="sxs-lookup"><span data-stu-id="7dce3-141">String collection</span></span>|<span data-ttu-id="7dce3-142">在继承自 [deviceManagementConfigurationSettingDefinition 上搜索设置的令牌](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="7dce3-143">infoUrls</span></span>|<span data-ttu-id="7dce3-144">字符串集合</span><span class="sxs-lookup"><span data-stu-id="7dce3-144">String collection</span></span>|<span data-ttu-id="7dce3-145">可以在"继承自[deviceManagementConfigurationSettingDefinition"](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)上找到链接列表，了解有关设置详细信息</span><span class="sxs-lookup"><span data-stu-id="7dce3-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="7dce3-146">occurrence</span></span>|[<span data-ttu-id="7dce3-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="7dce3-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="7dce3-148">指示设置是否必需。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="7dce3-149">baseUri</span></span>|<span data-ttu-id="7dce3-150">String</span><span class="sxs-lookup"><span data-stu-id="7dce3-150">String</span></span>|<span data-ttu-id="7dce3-151">基本 CSP 路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="7dce3-152">offsetUri</span></span>|<span data-ttu-id="7dce3-153">String</span><span class="sxs-lookup"><span data-stu-id="7dce3-153">String</span></span>|<span data-ttu-id="7dce3-154">从 Base 偏移 CSP 路径 继承 [自 deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7dce3-155">rootDefinitionId</span></span>|<span data-ttu-id="7dce3-156">String</span><span class="sxs-lookup"><span data-stu-id="7dce3-156">String</span></span>|<span data-ttu-id="7dce3-157">根设置定义（如果该设置是子设置）。</span><span class="sxs-lookup"><span data-stu-id="7dce3-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="7dce3-158">继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="7dce3-159">categoryId</span></span>|<span data-ttu-id="7dce3-160">String</span><span class="sxs-lookup"><span data-stu-id="7dce3-160">String</span></span>|<span data-ttu-id="7dce3-161">指定在 CSP) 从[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)的指定配置服务提供程序 (配置设置的区域组</span><span class="sxs-lookup"><span data-stu-id="7dce3-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="7dce3-162">settingUsage</span></span>|[<span data-ttu-id="7dce3-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="7dce3-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="7dce3-164">设置类型，例如，配置和合规性 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="7dce3-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="7dce3-165">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="7dce3-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="7dce3-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="7dce3-166">uxBehavior</span></span>|[<span data-ttu-id="7dce3-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="7dce3-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="7dce3-168">在 UX 中设置控件类型表示形式 继承 [自 deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="7dce3-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="7dce3-169">可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。</span><span class="sxs-lookup"><span data-stu-id="7dce3-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="7dce3-170">id</span><span class="sxs-lookup"><span data-stu-id="7dce3-170">id</span></span>|<span data-ttu-id="7dce3-171">String</span><span class="sxs-lookup"><span data-stu-id="7dce3-171">String</span></span>|<span data-ttu-id="7dce3-172">项的标识符 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-172">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-173">说明</span><span class="sxs-lookup"><span data-stu-id="7dce3-173">description</span></span>|<span data-ttu-id="7dce3-174">String</span><span class="sxs-lookup"><span data-stu-id="7dce3-174">String</span></span>|<span data-ttu-id="7dce3-175">项目说明 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-175">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-176">helpText</span><span class="sxs-lookup"><span data-stu-id="7dce3-176">helpText</span></span>|<span data-ttu-id="7dce3-177">String</span><span class="sxs-lookup"><span data-stu-id="7dce3-177">String</span></span>|<span data-ttu-id="7dce3-178">项的帮助文本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-178">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-179">名称</span><span class="sxs-lookup"><span data-stu-id="7dce3-179">name</span></span>|<span data-ttu-id="7dce3-180">String</span><span class="sxs-lookup"><span data-stu-id="7dce3-180">String</span></span>|<span data-ttu-id="7dce3-181">项目名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-181">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-182">displayName</span><span class="sxs-lookup"><span data-stu-id="7dce3-182">displayName</span></span>|<span data-ttu-id="7dce3-183">String</span><span class="sxs-lookup"><span data-stu-id="7dce3-183">String</span></span>|<span data-ttu-id="7dce3-184">项目的显示名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-184">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-185">version</span><span class="sxs-lookup"><span data-stu-id="7dce3-185">version</span></span>|<span data-ttu-id="7dce3-186">String</span><span class="sxs-lookup"><span data-stu-id="7dce3-186">String</span></span>|<span data-ttu-id="7dce3-187">项目版本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7dce3-187">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7dce3-188">选项</span><span class="sxs-lookup"><span data-stu-id="7dce3-188">options</span></span>|<span data-ttu-id="7dce3-189">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7dce3-189">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) collection</span></span>|<span data-ttu-id="7dce3-190">可以选择的设置选项</span><span class="sxs-lookup"><span data-stu-id="7dce3-190">Options for the setting that can be selected</span></span>|
|<span data-ttu-id="7dce3-191">defaultOptionId</span><span class="sxs-lookup"><span data-stu-id="7dce3-191">defaultOptionId</span></span>|<span data-ttu-id="7dce3-192">String</span><span class="sxs-lookup"><span data-stu-id="7dce3-192">String</span></span>|<span data-ttu-id="7dce3-193">选项设置的默认选项</span><span class="sxs-lookup"><span data-stu-id="7dce3-193">Default option for choice setting</span></span>|



## <a name="response"></a><span data-ttu-id="7dce3-194">响应</span><span class="sxs-lookup"><span data-stu-id="7dce3-194">Response</span></span>
<span data-ttu-id="7dce3-195">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7dce3-195">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dce3-196">示例</span><span class="sxs-lookup"><span data-stu-id="7dce3-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dce3-197">请求</span><span class="sxs-lookup"><span data-stu-id="7dce3-197">Request</span></span>
<span data-ttu-id="7dce3-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7dce3-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 9906

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingDefinition",
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
  "options": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition",
      "optionValue": {
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
      "itemId": "Item Id value",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value"
    }
  ],
  "defaultOptionId": "Default Option Id value"
}
```

### <a name="response"></a><span data-ttu-id="7dce3-199">响应</span><span class="sxs-lookup"><span data-stu-id="7dce3-199">Response</span></span>
<span data-ttu-id="7dce3-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7dce3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9955

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingDefinition",
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
  "id": "30b2258a-258a-30b2-8a25-b2308a25b230",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "options": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition",
      "optionValue": {
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
      "itemId": "Item Id value",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value"
    }
  ],
  "defaultOptionId": "Default Option Id value"
}
```




