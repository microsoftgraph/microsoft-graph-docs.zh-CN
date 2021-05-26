---
title: deviceManagementConfigurationStringSettingValue 资源类型
description: 简单设置值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e2374fd660fbfdcebee46ec6053d8ddc93f2010
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666700"
---
# <a name="devicemanagementconfigurationstringsettingvalue-resource-type"></a><span data-ttu-id="47258-103">deviceManagementConfigurationStringSettingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="47258-103">deviceManagementConfigurationStringSettingValue resource type</span></span>

<span data-ttu-id="47258-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47258-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47258-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47258-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47258-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47258-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47258-107">简单设置值</span><span class="sxs-lookup"><span data-stu-id="47258-107">Simple setting value</span></span>


<span data-ttu-id="47258-108">继承自 [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="47258-108">Inherits from [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47258-109">属性</span><span class="sxs-lookup"><span data-stu-id="47258-109">Properties</span></span>
|<span data-ttu-id="47258-110">属性</span><span class="sxs-lookup"><span data-stu-id="47258-110">Property</span></span>|<span data-ttu-id="47258-111">类型</span><span class="sxs-lookup"><span data-stu-id="47258-111">Type</span></span>|<span data-ttu-id="47258-112">说明</span><span class="sxs-lookup"><span data-stu-id="47258-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47258-113">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="47258-113">settingValueTemplateReference</span></span>|[<span data-ttu-id="47258-114">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="47258-114">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="47258-115">设置值模板引用 继承自 [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="47258-115">Setting value template reference Inherited from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>|
|<span data-ttu-id="47258-116">value</span><span class="sxs-lookup"><span data-stu-id="47258-116">value</span></span>|<span data-ttu-id="47258-117">String</span><span class="sxs-lookup"><span data-stu-id="47258-117">String</span></span>|<span data-ttu-id="47258-118">字符串设置的值。</span><span class="sxs-lookup"><span data-stu-id="47258-118">Value of the string setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47258-119">关系</span><span class="sxs-lookup"><span data-stu-id="47258-119">Relationships</span></span>
<span data-ttu-id="47258-120">无</span><span class="sxs-lookup"><span data-stu-id="47258-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47258-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47258-121">JSON Representation</span></span>
<span data-ttu-id="47258-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47258-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": "String"
}
```




