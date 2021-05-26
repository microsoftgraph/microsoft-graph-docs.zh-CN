---
title: deviceManagementConfigurationSimpleSettingCollectionInstance 资源类型
description: 简单设置集合实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30dcfb5d02aebb1e7bf346c6dd1f4b37e1103b49
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664921"
---
# <a name="devicemanagementconfigurationsimplesettingcollectioninstance-resource-type"></a><span data-ttu-id="0adfd-103">deviceManagementConfigurationSimpleSettingCollectionInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="0adfd-103">deviceManagementConfigurationSimpleSettingCollectionInstance resource type</span></span>

<span data-ttu-id="0adfd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0adfd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0adfd-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0adfd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0adfd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0adfd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0adfd-107">简单设置集合实例</span><span class="sxs-lookup"><span data-stu-id="0adfd-107">Simple setting collection instance</span></span>


<span data-ttu-id="0adfd-108">继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0adfd-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0adfd-109">属性</span><span class="sxs-lookup"><span data-stu-id="0adfd-109">Properties</span></span>
|<span data-ttu-id="0adfd-110">属性</span><span class="sxs-lookup"><span data-stu-id="0adfd-110">Property</span></span>|<span data-ttu-id="0adfd-111">类型</span><span class="sxs-lookup"><span data-stu-id="0adfd-111">Type</span></span>|<span data-ttu-id="0adfd-112">说明</span><span class="sxs-lookup"><span data-stu-id="0adfd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0adfd-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="0adfd-113">settingDefinitionId</span></span>|<span data-ttu-id="0adfd-114">String</span><span class="sxs-lookup"><span data-stu-id="0adfd-114">String</span></span>|<span data-ttu-id="0adfd-115">设置定义 ID 继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0adfd-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="0adfd-116">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="0adfd-116">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="0adfd-117">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="0adfd-117">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="0adfd-118">设置实例模板引用 继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0adfd-118">Setting Instance Template Reference Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="0adfd-119">simpleSettingCollectionValue</span><span class="sxs-lookup"><span data-stu-id="0adfd-119">simpleSettingCollectionValue</span></span>|<span data-ttu-id="0adfd-120">[deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0adfd-120">[deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md) collection</span></span>|<span data-ttu-id="0adfd-121">简单设置集合实例值</span><span class="sxs-lookup"><span data-stu-id="0adfd-121">Simple setting collection instance value</span></span>|

## <a name="relationships"></a><span data-ttu-id="0adfd-122">关系</span><span class="sxs-lookup"><span data-stu-id="0adfd-122">Relationships</span></span>
<span data-ttu-id="0adfd-123">无</span><span class="sxs-lookup"><span data-stu-id="0adfd-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0adfd-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0adfd-124">JSON Representation</span></span>
<span data-ttu-id="0adfd-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0adfd-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  },
  "simpleSettingCollectionValue": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
      "settingValueTemplateReference": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
        "settingValueTemplateId": "String",
        "useTemplateDefault": true
      },
      "value": "String"
    }
  ]
}
```




