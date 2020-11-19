---
title: deviceManagementConfigurationSetting 资源类型
description: 策略内的设置实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3767f7a9e21b72175f6df40dca78a0b2c0600b58
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241285"
---
# <a name="devicemanagementconfigurationsetting-resource-type"></a><span data-ttu-id="db02a-103">deviceManagementConfigurationSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="db02a-103">deviceManagementConfigurationSetting resource type</span></span>

<span data-ttu-id="db02a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db02a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db02a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db02a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db02a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db02a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db02a-107">策略内的设置实例</span><span class="sxs-lookup"><span data-stu-id="db02a-107">Setting instance within policy</span></span>

## <a name="methods"></a><span data-ttu-id="db02a-108">方法</span><span class="sxs-lookup"><span data-stu-id="db02a-108">Methods</span></span>
|<span data-ttu-id="db02a-109">方法</span><span class="sxs-lookup"><span data-stu-id="db02a-109">Method</span></span>|<span data-ttu-id="db02a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="db02a-110">Return Type</span></span>|<span data-ttu-id="db02a-111">说明</span><span class="sxs-lookup"><span data-stu-id="db02a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="db02a-112">列出 deviceManagementConfigurationSettings</span><span class="sxs-lookup"><span data-stu-id="db02a-112">List deviceManagementConfigurationSettings</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationsetting-list.md)|<span data-ttu-id="db02a-113">[deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db02a-113">[deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) collection</span></span>|<span data-ttu-id="db02a-114">列出 [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="db02a-114">List properties and relationships of the [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) objects.</span></span>|
|[<span data-ttu-id="db02a-115">获取 deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="db02a-115">Get deviceManagementConfigurationSetting</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationsetting-get.md)|[<span data-ttu-id="db02a-116">deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="db02a-116">deviceManagementConfigurationSetting</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|<span data-ttu-id="db02a-117">读取 [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="db02a-117">Read properties and relationships of the [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>|
|[<span data-ttu-id="db02a-118">创建 deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="db02a-118">Create deviceManagementConfigurationSetting</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationsetting-create.md)|[<span data-ttu-id="db02a-119">deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="db02a-119">deviceManagementConfigurationSetting</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|<span data-ttu-id="db02a-120">创建新的 [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db02a-120">Create a new [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>|
|[<span data-ttu-id="db02a-121">删除 deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="db02a-121">Delete deviceManagementConfigurationSetting</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationsetting-delete.md)|<span data-ttu-id="db02a-122">无</span><span class="sxs-lookup"><span data-stu-id="db02a-122">None</span></span>|<span data-ttu-id="db02a-123">删除 [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)。</span><span class="sxs-lookup"><span data-stu-id="db02a-123">Deletes a [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md).</span></span>|
|[<span data-ttu-id="db02a-124">更新 deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="db02a-124">Update deviceManagementConfigurationSetting</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationsetting-update.md)|[<span data-ttu-id="db02a-125">deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="db02a-125">deviceManagementConfigurationSetting</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|<span data-ttu-id="db02a-126">更新 [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="db02a-126">Update the properties of a [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="db02a-127">属性</span><span class="sxs-lookup"><span data-stu-id="db02a-127">Properties</span></span>
|<span data-ttu-id="db02a-128">属性</span><span class="sxs-lookup"><span data-stu-id="db02a-128">Property</span></span>|<span data-ttu-id="db02a-129">类型</span><span class="sxs-lookup"><span data-stu-id="db02a-129">Type</span></span>|<span data-ttu-id="db02a-130">说明</span><span class="sxs-lookup"><span data-stu-id="db02a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db02a-131">id</span><span class="sxs-lookup"><span data-stu-id="db02a-131">id</span></span>|<span data-ttu-id="db02a-132">String</span><span class="sxs-lookup"><span data-stu-id="db02a-132">String</span></span>|<span data-ttu-id="db02a-133">此设置在包含它的策略内的键。</span><span class="sxs-lookup"><span data-stu-id="db02a-133">Key of this setting within the policy which contains it.</span></span> <span data-ttu-id="db02a-134">自动生成。</span><span class="sxs-lookup"><span data-stu-id="db02a-134">Automatically generated.</span></span>|
|<span data-ttu-id="db02a-135">settingInstance</span><span class="sxs-lookup"><span data-stu-id="db02a-135">settingInstance</span></span>|[<span data-ttu-id="db02a-136">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="db02a-136">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="db02a-137">设置实例</span><span class="sxs-lookup"><span data-stu-id="db02a-137">Setting Instance</span></span>|

## <a name="relationships"></a><span data-ttu-id="db02a-138">关系</span><span class="sxs-lookup"><span data-stu-id="db02a-138">Relationships</span></span>
|<span data-ttu-id="db02a-139">关系</span><span class="sxs-lookup"><span data-stu-id="db02a-139">Relationship</span></span>|<span data-ttu-id="db02a-140">类型</span><span class="sxs-lookup"><span data-stu-id="db02a-140">Type</span></span>|<span data-ttu-id="db02a-141">说明</span><span class="sxs-lookup"><span data-stu-id="db02a-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db02a-142">settingDefinitions</span><span class="sxs-lookup"><span data-stu-id="db02a-142">settingDefinitions</span></span>|<span data-ttu-id="db02a-143">[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db02a-143">[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) collection</span></span>|<span data-ttu-id="db02a-144">相关设置定义的列表</span><span class="sxs-lookup"><span data-stu-id="db02a-144">List of related Setting Definitions</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db02a-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db02a-145">JSON Representation</span></span>
<span data-ttu-id="db02a-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db02a-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSetting",
  "id": "String (identifier)",
  "settingInstance": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
    "settingDefinitionId": "String",
    "choiceSettingValue": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
      "value": "String",
      "children": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
          "settingDefinitionId": "String",
          "choiceSettingValue": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
            "value": "String",
            "children": [
              {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                "settingDefinitionId": "String",
                "choiceSettingValue": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                  "value": "String",
                  "children": [
                    {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                      "settingDefinitionId": "String",
                      "choiceSettingValue": {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                        "value": "String",
                        "children": [
                          {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                            "settingDefinitionId": "String",
                            "choiceSettingValue": {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                              "value": "String",
                              "children": [
                                {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                  "settingDefinitionId": "String",
                                  "choiceSettingValue": {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                    "value": "String",
                                    "children": [
                                      {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                        "settingDefinitionId": "String",
                                        "choiceSettingValue": {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                          "value": "String",
                                          "children": [
                                            {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                              "settingDefinitionId": "String",
                                              "choiceSettingValue": {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                "value": "String",
                                                "children": [
                                                  {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                    "settingDefinitionId": "String",
                                                    "choiceSettingValue": {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                      "value": "String",
                                                      "children": [
                                                        {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                          "settingDefinitionId": "String",
                                                          "choiceSettingValue": {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                            "value": "String",
                                                            "children": [
                                                              {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                "settingDefinitionId": "String",
                                                                "choiceSettingValue": {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                  "value": "String",
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": null,
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
  }
}
```




