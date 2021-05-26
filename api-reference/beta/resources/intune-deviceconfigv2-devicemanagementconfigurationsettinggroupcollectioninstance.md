---
title: deviceManagementConfigurationSettingGroupCollectionInstance 资源类型
description: 在策略中设置实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af7bab6d165780c66a7f61ce0143be98bd0195b7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665614"
---
# <a name="devicemanagementconfigurationsettinggroupcollectioninstance-resource-type"></a><span data-ttu-id="b1fc4-103">deviceManagementConfigurationSettingGroupCollectionInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1fc4-103">deviceManagementConfigurationSettingGroupCollectionInstance resource type</span></span>

<span data-ttu-id="b1fc4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1fc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1fc4-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1fc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1fc4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1fc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1fc4-107">在策略中设置实例</span><span class="sxs-lookup"><span data-stu-id="b1fc4-107">Setting instance within policy</span></span>


<span data-ttu-id="b1fc4-108">继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b1fc4-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b1fc4-109">属性</span><span class="sxs-lookup"><span data-stu-id="b1fc4-109">Properties</span></span>
|<span data-ttu-id="b1fc4-110">属性</span><span class="sxs-lookup"><span data-stu-id="b1fc4-110">Property</span></span>|<span data-ttu-id="b1fc4-111">类型</span><span class="sxs-lookup"><span data-stu-id="b1fc4-111">Type</span></span>|<span data-ttu-id="b1fc4-112">说明</span><span class="sxs-lookup"><span data-stu-id="b1fc4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1fc4-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b1fc4-113">settingDefinitionId</span></span>|<span data-ttu-id="b1fc4-114">String</span><span class="sxs-lookup"><span data-stu-id="b1fc4-114">String</span></span>|<span data-ttu-id="b1fc4-115">设置定义 ID 继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b1fc4-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="b1fc4-116">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="b1fc4-116">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="b1fc4-117">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="b1fc4-117">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="b1fc4-118">设置实例模板引用 继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b1fc4-118">Setting Instance Template Reference Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1fc4-119">关系</span><span class="sxs-lookup"><span data-stu-id="b1fc4-119">Relationships</span></span>
<span data-ttu-id="b1fc4-120">无</span><span class="sxs-lookup"><span data-stu-id="b1fc4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1fc4-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1fc4-121">JSON Representation</span></span>
<span data-ttu-id="b1fc4-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1fc4-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  }
}
```




