---
title: deviceManagementReusablePolicySetting 资源类型
description: Graph可重用设置的模型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 221f3d592254c5eb5e052ad5a69604cd3ddf6955
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666637"
---
# <a name="devicemanagementreusablepolicysetting-resource-type"></a><span data-ttu-id="2f5d1-103">deviceManagementReusablePolicySetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f5d1-103">deviceManagementReusablePolicySetting resource type</span></span>

<span data-ttu-id="2f5d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f5d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f5d1-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f5d1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f5d1-107">Graph可重用设置的模型</span><span class="sxs-lookup"><span data-stu-id="2f5d1-107">Graph model for a reusable setting</span></span>

## <a name="methods"></a><span data-ttu-id="2f5d1-108">方法</span><span class="sxs-lookup"><span data-stu-id="2f5d1-108">Methods</span></span>
|<span data-ttu-id="2f5d1-109">方法</span><span class="sxs-lookup"><span data-stu-id="2f5d1-109">Method</span></span>|<span data-ttu-id="2f5d1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2f5d1-110">Return Type</span></span>|<span data-ttu-id="2f5d1-111">说明</span><span class="sxs-lookup"><span data-stu-id="2f5d1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2f5d1-112">列出 deviceManagementReusablePolicySettings</span><span class="sxs-lookup"><span data-stu-id="2f5d1-112">List deviceManagementReusablePolicySettings</span></span>](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-list.md)|<span data-ttu-id="2f5d1-113">[deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f5d1-113">[deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) collection</span></span>|<span data-ttu-id="2f5d1-114">列出 [deviceManagementReusablePolicySetting 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-114">List properties and relationships of the [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) objects.</span></span>|
|[<span data-ttu-id="2f5d1-115">获取 deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="2f5d1-115">Get deviceManagementReusablePolicySetting</span></span>](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-get.md)|[<span data-ttu-id="2f5d1-116">deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="2f5d1-116">deviceManagementReusablePolicySetting</span></span>](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|<span data-ttu-id="2f5d1-117">读取 [deviceManagementReusablePolicySetting 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-117">Read properties and relationships of the [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object.</span></span>|
|[<span data-ttu-id="2f5d1-118">创建 deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="2f5d1-118">Create deviceManagementReusablePolicySetting</span></span>](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-create.md)|[<span data-ttu-id="2f5d1-119">deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="2f5d1-119">deviceManagementReusablePolicySetting</span></span>](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|<span data-ttu-id="2f5d1-120">创建新的 [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-120">Create a new [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object.</span></span>|
|[<span data-ttu-id="2f5d1-121">删除 deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="2f5d1-121">Delete deviceManagementReusablePolicySetting</span></span>](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-delete.md)|<span data-ttu-id="2f5d1-122">无</span><span class="sxs-lookup"><span data-stu-id="2f5d1-122">None</span></span>|<span data-ttu-id="2f5d1-123">删除 [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-123">Deletes a [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md).</span></span>|
|[<span data-ttu-id="2f5d1-124">更新 deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="2f5d1-124">Update deviceManagementReusablePolicySetting</span></span>](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-update.md)|[<span data-ttu-id="2f5d1-125">deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="2f5d1-125">deviceManagementReusablePolicySetting</span></span>](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|<span data-ttu-id="2f5d1-126">更新 [deviceManagementReusablePolicySetting 对象](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-126">Update the properties of a [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object.</span></span>|
|[<span data-ttu-id="2f5d1-127">clone 操作</span><span class="sxs-lookup"><span data-stu-id="2f5d1-127">clone action</span></span>](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-clone.md)|[<span data-ttu-id="2f5d1-128">deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="2f5d1-128">deviceManagementReusablePolicySetting</span></span>](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|<span data-ttu-id="2f5d1-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2f5d1-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2f5d1-130">属性</span><span class="sxs-lookup"><span data-stu-id="2f5d1-130">Properties</span></span>
|<span data-ttu-id="2f5d1-131">属性</span><span class="sxs-lookup"><span data-stu-id="2f5d1-131">Property</span></span>|<span data-ttu-id="2f5d1-132">类型</span><span class="sxs-lookup"><span data-stu-id="2f5d1-132">Type</span></span>|<span data-ttu-id="2f5d1-133">说明</span><span class="sxs-lookup"><span data-stu-id="2f5d1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f5d1-134">id</span><span class="sxs-lookup"><span data-stu-id="2f5d1-134">id</span></span>|<span data-ttu-id="2f5d1-135">String</span><span class="sxs-lookup"><span data-stu-id="2f5d1-135">String</span></span>|<span data-ttu-id="2f5d1-136">系统生成的可重用设置 ID。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-136">system generated reusable setting id.</span></span>|
|<span data-ttu-id="2f5d1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2f5d1-137">displayName</span></span>|<span data-ttu-id="2f5d1-138">String</span><span class="sxs-lookup"><span data-stu-id="2f5d1-138">String</span></span>|<span data-ttu-id="2f5d1-139">由显示名称的可重用设置。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-139">reusable setting display name supplied by user.</span></span>|
|<span data-ttu-id="2f5d1-140">说明</span><span class="sxs-lookup"><span data-stu-id="2f5d1-140">description</span></span>|<span data-ttu-id="2f5d1-141">String</span><span class="sxs-lookup"><span data-stu-id="2f5d1-141">String</span></span>|<span data-ttu-id="2f5d1-142">由用户提供的可重用设置说明。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-142">reusable setting description supplied by user.</span></span>|
|<span data-ttu-id="2f5d1-143">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2f5d1-143">settingDefinitionId</span></span>|<span data-ttu-id="2f5d1-144">String</span><span class="sxs-lookup"><span data-stu-id="2f5d1-144">String</span></span>|<span data-ttu-id="2f5d1-145">与此可重用设置关联的设置定义 ID。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-145">setting definition id associated with this reusable setting.</span></span>|
|<span data-ttu-id="2f5d1-146">settingInstance</span><span class="sxs-lookup"><span data-stu-id="2f5d1-146">settingInstance</span></span>|[<span data-ttu-id="2f5d1-147">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="2f5d1-147">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="2f5d1-148">可重用的设置配置实例</span><span class="sxs-lookup"><span data-stu-id="2f5d1-148">reusable setting configuration instance</span></span>|
|<span data-ttu-id="2f5d1-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f5d1-149">createdDateTime</span></span>|<span data-ttu-id="2f5d1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f5d1-150">DateTimeOffset</span></span>|<span data-ttu-id="2f5d1-151">可重用设置创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-151">reusable setting creation date and time.</span></span> <span data-ttu-id="2f5d1-152">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-152">This property is read-only.</span></span>|
|<span data-ttu-id="2f5d1-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f5d1-153">lastModifiedDateTime</span></span>|<span data-ttu-id="2f5d1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f5d1-154">DateTimeOffset</span></span>|<span data-ttu-id="2f5d1-155">上次修改可重用设置的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-155">date and time when reusable setting was last modified.</span></span> <span data-ttu-id="2f5d1-156">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-156">This property is read-only.</span></span>|
|<span data-ttu-id="2f5d1-157">version</span><span class="sxs-lookup"><span data-stu-id="2f5d1-157">version</span></span>|<span data-ttu-id="2f5d1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="2f5d1-158">Int32</span></span>|<span data-ttu-id="2f5d1-159">可重复使用设置的版本号。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-159">version number for reusable setting.</span></span> <span data-ttu-id="2f5d1-160">有效值为 0 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-160">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="2f5d1-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-161">This property is read-only.</span></span>|
|<span data-ttu-id="2f5d1-162">referencingConfigurationPolicyCount</span><span class="sxs-lookup"><span data-stu-id="2f5d1-162">referencingConfigurationPolicyCount</span></span>|<span data-ttu-id="2f5d1-163">Int32</span><span class="sxs-lookup"><span data-stu-id="2f5d1-163">Int32</span></span>|<span data-ttu-id="2f5d1-164">引用当前可重用设置的配置策略计数。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-164">count of configuration policies referencing the current reusable setting.</span></span> <span data-ttu-id="2f5d1-165">有效值为 0 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-165">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="2f5d1-166">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-166">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f5d1-167">关系</span><span class="sxs-lookup"><span data-stu-id="2f5d1-167">Relationships</span></span>
|<span data-ttu-id="2f5d1-168">关系</span><span class="sxs-lookup"><span data-stu-id="2f5d1-168">Relationship</span></span>|<span data-ttu-id="2f5d1-169">类型</span><span class="sxs-lookup"><span data-stu-id="2f5d1-169">Type</span></span>|<span data-ttu-id="2f5d1-170">说明</span><span class="sxs-lookup"><span data-stu-id="2f5d1-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f5d1-171">referencingConfigurationPolicies</span><span class="sxs-lookup"><span data-stu-id="2f5d1-171">referencingConfigurationPolicies</span></span>|<span data-ttu-id="2f5d1-172">[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f5d1-172">[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) collection</span></span>|<span data-ttu-id="2f5d1-173">引用当前可重用设置的配置策略</span><span class="sxs-lookup"><span data-stu-id="2f5d1-173">configuration policies referencing the current reusable setting</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f5d1-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f5d1-174">JSON Representation</span></span>
<span data-ttu-id="2f5d1-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f5d1-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReusablePolicySetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReusablePolicySetting",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "settingDefinitionId": "String",
  "settingInstance": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
    "settingDefinitionId": "String",
    "settingInstanceTemplateReference": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
      "settingInstanceTemplateId": "String"
    },
    "choiceSettingValue": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
      "settingValueTemplateReference": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
        "settingValueTemplateId": "String",
        "useTemplateDefault": true
      },
      "value": "String",
      "children": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
          "settingDefinitionId": "String",
          "settingInstanceTemplateReference": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
            "settingInstanceTemplateId": "String"
          },
          "choiceSettingValue": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
            "settingValueTemplateReference": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
              "settingValueTemplateId": "String",
              "useTemplateDefault": true
            },
            "value": "String",
            "children": [
              {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                "settingDefinitionId": "String",
                "settingInstanceTemplateReference": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                  "settingInstanceTemplateId": "String"
                },
                "choiceSettingValue": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                  "settingValueTemplateReference": {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                    "settingValueTemplateId": "String",
                    "useTemplateDefault": true
                  },
                  "value": "String",
                  "children": [
                    {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                      "settingDefinitionId": "String",
                      "settingInstanceTemplateReference": {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                        "settingInstanceTemplateId": "String"
                      },
                      "choiceSettingValue": {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                        "settingValueTemplateReference": {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                          "settingValueTemplateId": "String",
                          "useTemplateDefault": true
                        },
                        "value": "String",
                        "children": [
                          {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                            "settingDefinitionId": "String",
                            "settingInstanceTemplateReference": {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                              "settingInstanceTemplateId": "String"
                            },
                            "choiceSettingValue": {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                              "settingValueTemplateReference": {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                "settingValueTemplateId": "String",
                                "useTemplateDefault": true
                              },
                              "value": "String",
                              "children": [
                                {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                  "settingDefinitionId": "String",
                                  "settingInstanceTemplateReference": {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                    "settingInstanceTemplateId": "String"
                                  },
                                  "choiceSettingValue": {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                    "settingValueTemplateReference": {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                      "settingValueTemplateId": "String",
                                      "useTemplateDefault": true
                                    },
                                    "value": "String",
                                    "children": [
                                      {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                        "settingDefinitionId": "String",
                                        "settingInstanceTemplateReference": {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                          "settingInstanceTemplateId": "String"
                                        },
                                        "choiceSettingValue": {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                          "settingValueTemplateReference": {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                            "settingValueTemplateId": "String",
                                            "useTemplateDefault": true
                                          },
                                          "value": "String",
                                          "children": [
                                            {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                              "settingDefinitionId": "String",
                                              "settingInstanceTemplateReference": {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                "settingInstanceTemplateId": "String"
                                              },
                                              "choiceSettingValue": {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                "settingValueTemplateReference": {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                  "settingValueTemplateId": "String",
                                                  "useTemplateDefault": true
                                                },
                                                "value": "String",
                                                "children": [
                                                  {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                    "settingDefinitionId": "String",
                                                    "settingInstanceTemplateReference": {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                      "settingInstanceTemplateId": "String"
                                                    },
                                                    "choiceSettingValue": {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                      "settingValueTemplateReference": {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                        "settingValueTemplateId": "String",
                                                        "useTemplateDefault": true
                                                      },
                                                      "value": "String",
                                                      "children": [
                                                        {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                          "settingDefinitionId": "String",
                                                          "settingInstanceTemplateReference": {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                            "settingInstanceTemplateId": "String"
                                                          },
                                                          "choiceSettingValue": {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                            "settingValueTemplateReference": {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                              "settingValueTemplateId": "String",
                                                              "useTemplateDefault": true
                                                            },
                                                            "value": "String",
                                                            "children": [
                                                              {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                "settingDefinitionId": "String",
                                                                "settingInstanceTemplateReference": {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                                  "settingInstanceTemplateId": "String"
                                                                },
                                                                "choiceSettingValue": {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                  "settingValueTemplateReference": {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                                    "settingValueTemplateId": "String",
                                                                    "useTemplateDefault": true
                                                                  },
                                                                  "value": "String",
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": null,
                                                                      "settingInstanceTemplateReference": null,
                                                                      "choiceSettingValue": null
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
    }
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "referencingConfigurationPolicyCount": 1024
}
```




