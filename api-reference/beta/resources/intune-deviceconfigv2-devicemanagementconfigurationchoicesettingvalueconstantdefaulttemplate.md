---
title: deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate 资源类型
description: 选项设置值常量默认模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b74dbf6552fda605708dbd5f197f5ee0167d2ac
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868442"
---
# <a name="devicemanagementconfigurationchoicesettingvalueconstantdefaulttemplate-resource-type"></a><span data-ttu-id="bc4b1-103">deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc4b1-103">deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate resource type</span></span>

<span data-ttu-id="bc4b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc4b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc4b1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bc4b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc4b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc4b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc4b1-107">选项设置值常量默认模板</span><span class="sxs-lookup"><span data-stu-id="bc4b1-107">Choice Setting Value Constant Default Template</span></span>


<span data-ttu-id="bc4b1-108">继承自 [deviceManagementConfigurationChoiceSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)</span><span class="sxs-lookup"><span data-stu-id="bc4b1-108">Inherits from [deviceManagementConfigurationChoiceSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc4b1-109">属性</span><span class="sxs-lookup"><span data-stu-id="bc4b1-109">Properties</span></span>
|<span data-ttu-id="bc4b1-110">属性</span><span class="sxs-lookup"><span data-stu-id="bc4b1-110">Property</span></span>|<span data-ttu-id="bc4b1-111">类型</span><span class="sxs-lookup"><span data-stu-id="bc4b1-111">Type</span></span>|<span data-ttu-id="bc4b1-112">说明</span><span class="sxs-lookup"><span data-stu-id="bc4b1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc4b1-113">settingDefinitionOptionId</span><span class="sxs-lookup"><span data-stu-id="bc4b1-113">settingDefinitionOptionId</span></span>|<span data-ttu-id="bc4b1-114">String</span><span class="sxs-lookup"><span data-stu-id="bc4b1-114">String</span></span>|<span data-ttu-id="bc4b1-115">默认常量值</span><span class="sxs-lookup"><span data-stu-id="bc4b1-115">Default Constant Value</span></span>|
|<span data-ttu-id="bc4b1-116">children</span><span class="sxs-lookup"><span data-stu-id="bc4b1-116">children</span></span>|<span data-ttu-id="bc4b1-117">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc4b1-117">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="bc4b1-118">选项子项</span><span class="sxs-lookup"><span data-stu-id="bc4b1-118">Option Children</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc4b1-119">关系</span><span class="sxs-lookup"><span data-stu-id="bc4b1-119">Relationships</span></span>
<span data-ttu-id="bc4b1-120">无</span><span class="sxs-lookup"><span data-stu-id="bc4b1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc4b1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc4b1-121">JSON Representation</span></span>
<span data-ttu-id="bc4b1-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc4b1-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate",
  "settingDefinitionOptionId": "String",
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
  ]
}
```




