---
title: deviceManagementConfigurationGroupSettingCollectionInstanceTemplate 资源类型
description: 组设置集合实例模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a1b4b750b69521a055f5c82004db28e0bf8b52b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868431"
---
# <a name="devicemanagementconfigurationgroupsettingcollectioninstancetemplate-resource-type"></a><span data-ttu-id="e5070-103">deviceManagementConfigurationGroupSettingCollectionInstanceTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5070-103">deviceManagementConfigurationGroupSettingCollectionInstanceTemplate resource type</span></span>

<span data-ttu-id="e5070-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5070-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5070-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5070-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5070-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5070-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5070-107">组设置集合实例模板</span><span class="sxs-lookup"><span data-stu-id="e5070-107">Group Setting Collection Instance Template</span></span>


<span data-ttu-id="e5070-108">继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e5070-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e5070-109">属性</span><span class="sxs-lookup"><span data-stu-id="e5070-109">Properties</span></span>
|<span data-ttu-id="e5070-110">属性</span><span class="sxs-lookup"><span data-stu-id="e5070-110">Property</span></span>|<span data-ttu-id="e5070-111">类型</span><span class="sxs-lookup"><span data-stu-id="e5070-111">Type</span></span>|<span data-ttu-id="e5070-112">说明</span><span class="sxs-lookup"><span data-stu-id="e5070-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5070-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="e5070-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="e5070-114">String</span><span class="sxs-lookup"><span data-stu-id="e5070-114">String</span></span>|<span data-ttu-id="e5070-115">设置实例模板 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e5070-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="e5070-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e5070-116">settingDefinitionId</span></span>|<span data-ttu-id="e5070-117">String</span><span class="sxs-lookup"><span data-stu-id="e5070-117">String</span></span>|<span data-ttu-id="e5070-118">设置定义 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e5070-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="e5070-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="e5070-119">isRequired</span></span>|<span data-ttu-id="e5070-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5070-120">Boolean</span></span>|<span data-ttu-id="e5070-121">指示策略是否必须指定此设置。</span><span class="sxs-lookup"><span data-stu-id="e5070-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="e5070-122">继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e5070-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="e5070-123">groupSettingCollectionValueTemplate</span><span class="sxs-lookup"><span data-stu-id="e5070-123">groupSettingCollectionValueTemplate</span></span>|<span data-ttu-id="e5070-124">[deviceManagementConfigurationGroupSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvaluetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5070-124">[deviceManagementConfigurationGroupSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvaluetemplate.md) collection</span></span>|<span data-ttu-id="e5070-125">组设置集合值模板</span><span class="sxs-lookup"><span data-stu-id="e5070-125">Group Setting Collection Value Template</span></span>|
|<span data-ttu-id="e5070-126">allowUnmanagedValues</span><span class="sxs-lookup"><span data-stu-id="e5070-126">allowUnmanagedValues</span></span>|<span data-ttu-id="e5070-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5070-127">Boolean</span></span>|<span data-ttu-id="e5070-128">链接策略可能会追加模板中不存在的值。</span><span class="sxs-lookup"><span data-stu-id="e5070-128">Linked policy may append values which are not present in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5070-129">关系</span><span class="sxs-lookup"><span data-stu-id="e5070-129">Relationships</span></span>
<span data-ttu-id="e5070-130">无</span><span class="sxs-lookup"><span data-stu-id="e5070-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5070-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5070-131">JSON Representation</span></span>
<span data-ttu-id="e5070-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5070-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "groupSettingCollectionValueTemplate": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate",
      "children": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
          "settingInstanceTemplateId": "String",
          "settingDefinitionId": "String",
          "isRequired": true,
          "simpleSettingValueTemplate": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
            "settingValueTemplateId": "String"
          }
        }
      ],
      "settingValueTemplateId": "String"
    }
  ],
  "allowUnmanagedValues": true
}
```




