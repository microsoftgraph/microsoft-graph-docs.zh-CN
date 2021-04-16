---
title: deviceManagementConfigurationOptionDefinitionTemplate 资源类型
description: 选项定义模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d5c980882815b350db9c3571f7436a7921a6d278
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868427"
---
# <a name="devicemanagementconfigurationoptiondefinitiontemplate-resource-type"></a><span data-ttu-id="393c9-103">deviceManagementConfigurationOptionDefinitionTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="393c9-103">deviceManagementConfigurationOptionDefinitionTemplate resource type</span></span>

<span data-ttu-id="393c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="393c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="393c9-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="393c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="393c9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="393c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="393c9-107">选项定义模板</span><span class="sxs-lookup"><span data-stu-id="393c9-107">Option Definition Template</span></span>

## <a name="properties"></a><span data-ttu-id="393c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="393c9-108">Properties</span></span>
|<span data-ttu-id="393c9-109">属性</span><span class="sxs-lookup"><span data-stu-id="393c9-109">Property</span></span>|<span data-ttu-id="393c9-110">类型</span><span class="sxs-lookup"><span data-stu-id="393c9-110">Type</span></span>|<span data-ttu-id="393c9-111">说明</span><span class="sxs-lookup"><span data-stu-id="393c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="393c9-112">itemId</span><span class="sxs-lookup"><span data-stu-id="393c9-112">itemId</span></span>|<span data-ttu-id="393c9-113">String</span><span class="sxs-lookup"><span data-stu-id="393c9-113">String</span></span>|<span data-ttu-id="393c9-114">Option ItemId</span><span class="sxs-lookup"><span data-stu-id="393c9-114">Option ItemId</span></span>|
|<span data-ttu-id="393c9-115">children</span><span class="sxs-lookup"><span data-stu-id="393c9-115">children</span></span>|<span data-ttu-id="393c9-116">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="393c9-116">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="393c9-117">选项子项</span><span class="sxs-lookup"><span data-stu-id="393c9-117">Option Children</span></span>|

## <a name="relationships"></a><span data-ttu-id="393c9-118">关系</span><span class="sxs-lookup"><span data-stu-id="393c9-118">Relationships</span></span>
<span data-ttu-id="393c9-119">无</span><span class="sxs-lookup"><span data-stu-id="393c9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="393c9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="393c9-120">JSON Representation</span></span>
<span data-ttu-id="393c9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="393c9-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
  "itemId": "String",
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




