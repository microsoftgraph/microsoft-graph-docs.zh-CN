---
title: deviceManagementConfigurationSimpleSettingInstance 资源类型
description: 简单设置实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6c815ec0b90211ede9429abe707856af27ed79b5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666721"
---
# <a name="devicemanagementconfigurationsimplesettinginstance-resource-type"></a><span data-ttu-id="5ea4f-103">deviceManagementConfigurationSimpleSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ea4f-103">deviceManagementConfigurationSimpleSettingInstance resource type</span></span>

<span data-ttu-id="5ea4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ea4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ea4f-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ea4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ea4f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ea4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ea4f-107">简单设置实例</span><span class="sxs-lookup"><span data-stu-id="5ea4f-107">Simple setting instance</span></span>


<span data-ttu-id="5ea4f-108">继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5ea4f-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5ea4f-109">属性</span><span class="sxs-lookup"><span data-stu-id="5ea4f-109">Properties</span></span>
|<span data-ttu-id="5ea4f-110">属性</span><span class="sxs-lookup"><span data-stu-id="5ea4f-110">Property</span></span>|<span data-ttu-id="5ea4f-111">类型</span><span class="sxs-lookup"><span data-stu-id="5ea4f-111">Type</span></span>|<span data-ttu-id="5ea4f-112">说明</span><span class="sxs-lookup"><span data-stu-id="5ea4f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ea4f-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5ea4f-113">settingDefinitionId</span></span>|<span data-ttu-id="5ea4f-114">String</span><span class="sxs-lookup"><span data-stu-id="5ea4f-114">String</span></span>|<span data-ttu-id="5ea4f-115">设置定义 ID 继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5ea4f-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="5ea4f-116">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="5ea4f-116">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="5ea4f-117">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="5ea4f-117">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="5ea4f-118">设置实例模板引用 继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5ea4f-118">Setting Instance Template Reference Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="5ea4f-119">simpleSettingValue</span><span class="sxs-lookup"><span data-stu-id="5ea4f-119">simpleSettingValue</span></span>|[<span data-ttu-id="5ea4f-120">deviceManagementConfigurationSimpleSettingValue</span><span class="sxs-lookup"><span data-stu-id="5ea4f-120">deviceManagementConfigurationSimpleSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)|<span data-ttu-id="5ea4f-121">简单设置实例值</span><span class="sxs-lookup"><span data-stu-id="5ea4f-121">Simple setting instance value</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ea4f-122">关系</span><span class="sxs-lookup"><span data-stu-id="5ea4f-122">Relationships</span></span>
<span data-ttu-id="5ea4f-123">无</span><span class="sxs-lookup"><span data-stu-id="5ea4f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ea4f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ea4f-124">JSON Representation</span></span>
<span data-ttu-id="5ea4f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ea4f-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  },
  "simpleSettingValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
    "settingValueTemplateReference": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
      "settingValueTemplateId": "String",
      "useTemplateDefault": true
    },
    "value": "String"
  }
}
```




