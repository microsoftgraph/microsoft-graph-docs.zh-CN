---
title: deviceManagementConfigurationChoiceSettingValueDefinitionTemplate 资源类型
description: 选项设置值定义模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b4caada35c50a0d3e804a66f1556f13fbc88bfa
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868436"
---
# <a name="devicemanagementconfigurationchoicesettingvaluedefinitiontemplate-resource-type"></a><span data-ttu-id="7de31-103">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="7de31-103">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate resource type</span></span>

<span data-ttu-id="7de31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7de31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7de31-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7de31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7de31-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7de31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7de31-107">选项设置值定义模板</span><span class="sxs-lookup"><span data-stu-id="7de31-107">Choice Setting Value Definition Template</span></span>

## <a name="properties"></a><span data-ttu-id="7de31-108">属性</span><span class="sxs-lookup"><span data-stu-id="7de31-108">Properties</span></span>
|<span data-ttu-id="7de31-109">属性</span><span class="sxs-lookup"><span data-stu-id="7de31-109">Property</span></span>|<span data-ttu-id="7de31-110">类型</span><span class="sxs-lookup"><span data-stu-id="7de31-110">Type</span></span>|<span data-ttu-id="7de31-111">说明</span><span class="sxs-lookup"><span data-stu-id="7de31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7de31-112">allowedOptions</span><span class="sxs-lookup"><span data-stu-id="7de31-112">allowedOptions</span></span>|<span data-ttu-id="7de31-113">[deviceManagementConfigurationOptionDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinitiontemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7de31-113">[deviceManagementConfigurationOptionDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinitiontemplate.md) collection</span></span>|<span data-ttu-id="7de31-114">选项设置允许的选项</span><span class="sxs-lookup"><span data-stu-id="7de31-114">Choice Setting Allowed Options</span></span>|

## <a name="relationships"></a><span data-ttu-id="7de31-115">关系</span><span class="sxs-lookup"><span data-stu-id="7de31-115">Relationships</span></span>
<span data-ttu-id="7de31-116">无</span><span class="sxs-lookup"><span data-stu-id="7de31-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7de31-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7de31-117">JSON Representation</span></span>
<span data-ttu-id="7de31-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7de31-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
  "allowedOptions": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
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
  ]
}
```




